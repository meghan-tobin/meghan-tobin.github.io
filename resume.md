---
layout: about
title: Resume
---

{% assign resume_pdf = "/assets/images/MeghanTobinResume2026.pdf" %}
{% comment %} The ?v= changes on every build so browsers fetch the newest PDF instead of a cached one. {% endcomment %}
{% capture resume_pdf %}{{ resume_pdf }}?v={{ site.time | date: "%s" }}{% endcapture %}

<div class="resume-wrap">
  <a href="{{ resume_pdf }}" class="resume-download" download="MeghanTobinResume.pdf">
    <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>
    Download
  </a>
  <div class="resume-pages" id="resume-pages" data-pdf="{{ resume_pdf }}">
    <noscript><p><a href="{{ resume_pdf }}">Open the resume</a></p></noscript>
  </div>
</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/pdf.js/3.11.174/pdf.min.js"></script>
<script>
  (function () {
    var container = document.getElementById('resume-pages');
    var url = container.dataset.pdf;
    var fallback = '<p class="resume-fallback"><a href="' + url + '" target="_blank" rel="noopener">Open the resume</a></p>';
    if (!window.pdfjsLib) { container.innerHTML = fallback; return; }
    pdfjsLib.GlobalWorkerOptions.workerSrc =
      'https://cdnjs.cloudflare.com/ajax/libs/pdf.js/3.11.174/pdf.worker.min.js';

    var pdfDoc = null;

    // Draw every page as a canvas sized to the column width (sharp on retina screens).
    function render() {
      container.innerHTML = '';
      var width = container.clientWidth;
      var dpr = window.devicePixelRatio || 1;
      var chain = Promise.resolve();
      for (var n = 1; n <= pdfDoc.numPages; n++) {
        (function (num) {
          chain = chain.then(function () { return pdfDoc.getPage(num); }).then(function (page) {
            var base = page.getViewport({ scale: 1 });
            var viewport = page.getViewport({ scale: (width / base.width) * dpr });
            var canvas = document.createElement('canvas');
            canvas.className = 'resume-page';
            canvas.width = viewport.width;
            canvas.height = viewport.height;
            container.appendChild(canvas);
            return page.render({ canvasContext: canvas.getContext('2d'), viewport: viewport }).promise;
          });
        })(n);
      }
      return chain;
    }

    pdfjsLib.getDocument(url).promise.then(function (doc) {
      pdfDoc = doc;
      return render();
    }).catch(function () { container.innerHTML = fallback; });

    var lastWidth = container.clientWidth, timer;
    window.addEventListener('resize', function () {
      clearTimeout(timer);
      timer = setTimeout(function () {
        if (pdfDoc && container.clientWidth !== lastWidth) {
          lastWidth = container.clientWidth;
          render();
        }
      }, 200);
    });
  })();
</script>
