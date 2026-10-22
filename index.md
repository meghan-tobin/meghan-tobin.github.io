---
layout: home
---

<div class="about-hero">
  <img src="/assets/images/web/gate.jpg" alt="Meghan Tobin" class="about-photo">
  <div class="about-bio">
    <h1>Hi, I'm Meghan!</h1>
    <p>
       I'm a Software Engineer based in San Francisco. I'm originally from Boston, but I moved to California after graduating from the University of Illinois Urbana-Champaign with a degree in Computer Science!
       <br><br>
       Since graduating, I've enjoyed working as a Software Engineer and tackling a wide range of technical challenges. I've always loved problem-solving, but through my experience, I've discovered that I'm especially drawn to larger-scale problems that require collaboration, thoughtful decision-making, and finding solutions that work for everyone involved.
       <br><br>
       I'm excited to keep learning, take on new challenges, and apply my technical background to building products that solve meaningful problems. I'm particularly interested in opportunities where I can combine technical problem-solving with collaboration and a broader perspective on how products are built.
    </p>
  </div>
</div>

<div class="dashed"></div>

<div class="bubble-row">
  <button type="button" class="bubble bubble-square bubble-edu" aria-expanded="false" aria-controls="bubble-panel-edu">
    <svg class="bubble-icon" width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="M22 10 12 5 2 10l10 5 10-5z"/><path d="M6 12v5c0 1.1 2.7 3 6 3s6-1.9 6-3v-5"/><path d="M22 10v6"/></svg>
    <span class="bubble-label">Education</span>
    <span class="bubble-title">University of Illinois Urbana-Champaign</span>
    <span class="bubble-sub">Bachelor of Science in Computer Science</span>
    <span class="bubble-date">2020 – 2023</span>
  </button>

  <div class="bubble-panel" id="bubble-panel-edu" hidden>
    <p>I studied Computer Science at the University of Illinois Urbana-Champaign and loved my time there, especially getting involved in cybersecurity clubs on campus. I-L-L!</p>
    <a href="/resume" class="bubble-panel-link">View resume &rarr;</a>
  </div>

  <button type="button" class="bubble bubble-square" aria-expanded="false" aria-controls="bubble-panel-everfox">
    <span class="bubble-label">Experience</span>
    <span class="bubble-title">Everfox</span>
    <span class="bubble-roles">
      <span class="bubble-role"><span>Software Engineering Intern</span><span class="bubble-date">May 2023- December 2023</span></span>
      <span class="bubble-arrow" aria-hidden="true"><svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><line x1="12" y1="4" x2="12" y2="20"/><polyline points="6 14 12 20 18 14"/></svg></span>
      <span class="bubble-role"><span>Software Engineer I</span><span class="bubble-date">January 2024 – Janurary 2025</span></span>
      <span class="bubble-arrow" aria-hidden="true"><svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><line x1="12" y1="4" x2="12" y2="20"/><polyline points="6 14 12 20 18 14"/></svg></span>
      <span class="bubble-role"><span>Software Engineer II</span><span class="bubble-date">Janurary 2025 – Present</span></span>
    </span>
  </button>

  <div class="bubble-panel" id="bubble-panel-everfox" hidden>
    <p>I started at Everfox as an intern on the Trusted Thin Client team, working on customer-driven projects to improve the user experience when working across different security classification levels. I also began developing a hardware testing suite that I later led as an intern project, which was ultimately adopted by the testing organization.</p>
    <p>After joining full-time, I took on broader responsibilities, from organizing and expanding the company's internship program to leading the development and rollout of Magic Mirror. I worked closely with teams across engineering to understand their needs, shape the product's direction, and guide it from an early proof of concept to a tool relied on across the organization. Through these experiences, I discovered how much I enjoy not just solving technical problems, but also figuring out what needs to be built, bringing people together, and guiding projects from idea to execution.</p>
    <a href="/resume" class="bubble-panel-link">View resume &rarr;</a>
  </div>

  <button type="button" class="bubble bubble-square" aria-expanded="false" aria-controls="bubble-panel-ml">
    <span class="bubble-label">Experience</span>
    <span class="bubble-title">ML / AI</span>
    <span class="bubble-roles">
      <span class="bubble-role"><span>Machine Learning Intern &middot; Pointerra3D</span><span class="bubble-date">May 2021 – May 2023</span></span>
      <span class="bubble-arrow" aria-hidden="true"><svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><line x1="12" y1="4" x2="12" y2="20"/><polyline points="6 14 12 20 18 14"/></svg></span>
      <span class="bubble-role"><span>Machine Learning Consultant &middot; Private Client</span><span class="bubble-date">September 2025 – January 2026</span></span>
    </span>
  </button>

  <div class="bubble-panel" id="bubble-panel-ml" hidden>
    <p>I started working as a Machine Learning Intern at Pointerra3D in college. I got to explore how machine learning could be used to understand and predict changes in 3D vegetation data. I worked on everything from preparing the data to experimenting with different models, and was able to greatly improve prediction accuracy. I also built a tool to turn the results into 3D visualizations, making it easier to see what the models were predicting.</p>
    <p>A few years later I was asked to consult for a startup founded by a former colleague, where I was tasked with defining the machine learning strategy for a new project. I worked with the technical lead to understand the business goals and technical constraints, evaluate different approaches, and determine the best direction for the product. By testing and comparing potential solutions, I developed a recommendation and roadmap to guide the project toward production</p>
    <a href="/resume" class="bubble-panel-link">View resume &rarr;</a>
  </div>
</div>

<script>
  (function () {
    var cards = document.querySelectorAll('.bubble-row .bubble');
    cards.forEach(function (card) {
      card.addEventListener('click', function () {
        var opening = card.getAttribute('aria-expanded') !== 'true';
        cards.forEach(function (c) {
          c.setAttribute('aria-expanded', 'false');
          document.getElementById(c.getAttribute('aria-controls')).hidden = true;
        });
        if (opening) {
          card.setAttribute('aria-expanded', 'true');
          document.getElementById(card.getAttribute('aria-controls')).hidden = false;
        }
      });
    });
  })();
</script>

<div class="dashed"></div>

## Hobbies

<div class="hobby-chips">
  <span 
    class="tag hobby-tag" 
    data-info="I grew up swimming competitively, and I still spend a lot of my free time in the pool. I usually swim after work and love meeting other swimmers or convincing friends to give it a try. I'm currently training for a marathon swim in Tahoe and trying to swim in the Bay more frequently." 
    data-photo="/assets/images/web/swim.jpg">Swimming
  </span>

  <span 
    class="tag hobby-tag" 
    data-info="I started making jewelry a few years ago because I wanted a new craft to do. I mostly make earrings and do jewelry repairs for friends and family. I've thought about eventually making my own collection, which is actually what inspired me to build Bijoux Breakdown!" 
    data-photo="/assets/images/web/earring.jpg">Jewelry
  </span>

  <span 
    class="tag hobby-tag" 
    data-info="I recently started running, and it has quickly become one of my favorite hobbies. I enjoy runs along Marina Green and Ocean Beach. I just ran my first 10K, and I’m gradually building up to longer distances!" 
    data-photo="/assets/images/web/run.jpg">Running
  </span>

  <span 
    class="tag hobby-tag" 
    data-info="I met a lot of my friends through Volo. We've played a lot of sports at this point, but had surprising success in dodgeball! " 
    data-photo="/assets/images/web/volo.jpg">Volo
  </span>

  <span 
    class="tag hobby-tag" 
    data-info="I love baking and recently purchased a KitchenAid mixer, which has caused me to bake even more. I've gotten into the habit of baking pretty much every week and bringing treats to my friends and roommates. Tiramisu and anything pumpkin-flavored are probably my favorites to make." 
    data-photo="/assets/images/web/tiramisu.jpg">Baking
  </span>

  <span 
    class="tag hobby-tag" 
    data-info="I adopted Luna a few years ago and it's one of the bes decisions I've ever made. She's super cute and wins over everyone she meets. We spend time playing with her favorite mouse toys, watching birds from our balcony, and going on occasional outdoor adventures." 
    data-photo="/assets/images/web/luna6.jpg">Luna
  </span>
</div>

<div class="hobby-detail" id="hobby-detail">
  <img class="hobby-detail-photo" id="hobby-detail-photo" src="" alt="">
  <div class="hobby-detail-text" id="hobby-detail-text"></div>
</div>

<script>
(function () {
  // Hobby detail panel
  var detail = document.getElementById('hobby-detail');
  var detailPhoto = document.getElementById('hobby-detail-photo');
  var detailText = document.getElementById('hobby-detail-text');
  var activeChip = null;

  document.querySelectorAll('.hobby-tag').forEach(function (chip) {
    chip.addEventListener('click', function (e) {
      e.stopPropagation();

      if (activeChip === this && detail.classList.contains('visible')) {
        detail.classList.remove('visible');
        this.classList.remove('hobby-tag-active');
        activeChip = null;
        return;
      }

      if (activeChip) activeChip.classList.remove('hobby-tag-active');
      activeChip = this;
      this.classList.add('hobby-tag-active');

      var photo = this.dataset.photo;
      if (photo) {
        detailPhoto.src = photo;
        detailPhoto.style.display = 'block';
      } else {
        detailPhoto.style.display = 'none';
      }
      if (this.dataset.tall) {
        detailPhoto.classList.add('hobby-detail-photo--tall');
      } else {
        detailPhoto.classList.remove('hobby-detail-photo--tall');
      }
      detailText.textContent = this.dataset.info;
      detail.classList.add('visible');
    });
  });

})();
</script>
