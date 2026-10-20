---
layout: home
---

<div class="about-hero">
  <img src="/assets/images/gate.png" alt="Meghan Tobin" class="about-photo">
  <div class="about-bio">
    <h1>Hi, I'm Meghan!</h1>
    <p>
       I'm a Software Engineer based in San Francisco. I'm originally from Boston, but I decided to leave the cold winters behind and move to California after graduating from the University of Illinois Urbana-Champaign with a degree in Computer Science!
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
    <p>I studied Computer Science at the University of Illinois Urbana-Champaign. I entered college with very little coding experience, but it didn't take long for me to realize I had found the right field. I was fascinated by the wide range of applications for computer science and the endless opportunities to solve meaningful problems. During my time at UIUC, I developed a particular interest in cybersecurity and became actively involved in cybersecurity organizations on campus.</p>
    <a href="/resume" class="bubble-panel-link">View full resume &rarr;</a>
  </div>

  <button type="button" class="bubble bubble-square" aria-expanded="false" aria-controls="bubble-panel-everfox">
    <span class="bubble-label">Experience</span>
    <span class="bubble-title">Everfox</span>
    <span class="bubble-roles">
      <span class="bubble-role"><span>Software Engineer II</span><span class="bubble-date">2025 – Present</span></span>
      <span class="bubble-role"><span>Software Engineer I</span><span class="bubble-date">2024 – 2025</span></span>
      <span class="bubble-role"><span>Software Engineering Intern</span><span class="bubble-date">Summer 2023</span></span>
    </span>
  </button>

  <div class="bubble-panel" id="bubble-panel-everfox" hidden>
    <h4>Software Engineer II</h4>
    <p>My focus shifted toward platform ownership and large-scale system rollout. I led the transformation of a proof-of-concept codebase into a mission-critical platform, defining architecture improvements, rollout strategy, and engineering standards while mentoring interns and driving feature development under aggressive timelines. I partnered with over 10 engineering teams to drive migration readiness, coordinate dependencies, and manage rollout execution, ensuring successful adoption across the organization. I also built operational dashboards and training systems to support migration monitoring, self-serve debugging, and end-to-end platform usage.</p>
    <h4>Software Engineer I</h4>
    <p>I moved into low-level systems and platform work across multiple engineering teams. I contributed to security hardening through seccomp-based compliance validation, improved system reliability through cross-product bug fixing, and integrated Coverity into the CI and developer toolchain to enable automated static analysis across the organization. I also operated and helped scale a newly established internship program, and led the largest intern project end-to-end, delivering a production-used hardware testing system and establishing execution standards for future cohorts.</p>
    <h4>Software Engineering Intern</h4>
    <p>I worked on two main projects spanning user-facing system improvements and hardware qualification workflows. One focused on building security-aware UI signals for RGB keyboards using D-Bus and Python, designed to reduce user error when switching between data classification levels. The second was a more open-ended hardware qualification problem, where I was responsible for defining project requirements and independently designing a solution approach.</p>
    <a href="/resume" class="bubble-panel-link">View full resume &rarr;</a>
  </div>

  <button type="button" class="bubble bubble-square" aria-expanded="false" aria-controls="bubble-panel-ml">
    <span class="bubble-label">Experience</span>
    <span class="bubble-title">ML / AI</span>
    <span class="bubble-roles">
      <span class="bubble-role"><span>Machine Learning Consultant &middot; Private Client</span><span class="bubble-date">2025 – 2026</span></span>
      <span class="bubble-role"><span>Machine Learning Intern &middot; Pointerra3D</span><span class="bubble-date">2022 – 2023</span></span>
    </span>
  </button>

  <div class="bubble-panel" id="bubble-panel-ml" hidden>
    <h4>Machine Learning Consultant &middot; Private Client</h4>
    <p>My work as an intern led me directly into a client engagement when a former engineering director founded a startup and brought me on as a machine learning consultant. I worked closely with a client director to define the ML problem space for voxelized LiDAR classification, translating system constraints into a structured modeling strategy. I designed and executed experiments across multiple machine learning approaches, benchmarking model performance under real-world dataset constraints, then synthesized results into a recommended implementation and deployment roadmap.</p>
    <h4>Machine Learning Intern &middot; Pointerra3D</h4>
    <p>I applied machine learning to 3D vegetation data. I built a data pipeline that converted 3D vegetation datasets into PostgreSQL tables hosted on AWS, enabling structured querying for model training. I trained and evaluated multiple regression models including Random Forest, Decision Tree, and Lasso Regression to predict vegetation growth over time, improving model performance from 72% to 98% accuracy and reducing regression runtime to under one minute. I also developed a Python-based visualization tool that converted CSV outputs into 3D models for interpreting predicted growth patterns.</p>
    <a href="/resume" class="bubble-panel-link">View full resume &rarr;</a>
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
    data-info="I grew up swimming competitively, and it remains one of my favorite activities. I swim regularly after work and am always looking to connect with other swimmers or encourage people to get into the sport. That led me to join SF Tsunami, which has become my current swim group in San Francisco. My primary stroke is butterfly, and I’m currently working toward open-water swimming in the Bay." 
    data-photo="/assets/images/swim.JPG">Swimming
  </span>

  <span 
    class="tag hobby-tag" 
    data-info="I started making jewelry a few years ago after realizing I wanted a more hands-on creative outlet in my life. I learned to design and create a variety of pieces, but earrings quickly became my favorite. Over time, I’ve made many of the earrings I wear today myself. That interest eventually grew into the idea of creating a small collection, which inspired my Bijoux Breakdown project!" 
    data-photo="/assets/images/earring.png">Jewelry
  </span>

  <span 
    class="tag hobby-tag" 
    data-info="I recently started running, and it has quickly become one of my favorite hobbies. I enjoy long runs around Marina Green and along Ocean Beach/Golden gate park. My next race is the San Francisco Alexi Pappas 10K, and I’m gradually building up to longer distances" 
    data-photo="/assets/images/run.png">Running
  </span>

  <span 
    class="tag hobby-tag" 
    data-info="I met many of my friends through Volo, which has become a consistent highlight of my week. I especially enjoyed Volo dodgeball, and my friend group has since started our own weekly version where we rotate through different sports." 
    data-photo="/assets/images/volo.jpg">Volo
  </span>

  <span 
    class="tag hobby-tag" 
    data-info="I love baking and recently started using a KitchenAid mixer, which has turned it into a weekly hobby. I often bake for friends and roommates and usually end up sharing most of what I make. My favorite desserts to make are tiramisu and anything pumpkin-flavored." 
    data-photo="/assets/images/tiramisu.jpeg">Baking
  </span>

  <span 
    class="tag hobby-tag" 
    data-info="I have a beloved cat named Luna, who I adopted two years ago. She is extremely affectionate and loved by everyone who meets her. We spend time playing with her favorite mouse toys, watching birds from our balcony, and going on occasional outdoor adventures." 
    data-photo="/assets/images/luna6.JPG">Luna
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
