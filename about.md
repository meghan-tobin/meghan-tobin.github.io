---
layout: about
title: About
---

<div class="about-hero">
  <img src="/assets/images/gate.png" alt="Meghan Tobin" class="about-photo">
  <div class="about-bio">
    <h1>Hi, I'm Meghan!</h1>
    <p>
       I'm a Software Engineer based in San Francisco. I'm originally from Boston, but I decided to leave the cold winters behind and move to California after graduating from from the University of Illinois Urbana-Champaign with a degree in Computer Science!
       <br><br>
       My interest in Computer Science began in high school. I always enjoyed math, and one of my teachers encouraged me to explore programming. I entered college with very little coding experience, but it didn't take long for me to realize I had found the right field. I was fascinated by the wide range of applications for computer science and the endless opportunities to solve meaningful problems. During my time at UIUC, I developed a particular interest in cybersecurity and became actively involved in cybersecurity organizations on campus.
       <br><br>
       While I enjoy the technical challenge of software engineering, I found myself increasingly drawn to the collaborative side of building products. Throughout my career, I've worked closely with engineers, product teams, interns, and stakeholders to define requirements, scope projects, create learning programs, and guide initiatives from concept to implementation. These experiences showed me that my greatest strengths lie not only in developing technical solutions, but also in aligning people around a common goal, communicating complex ideas clearly, and helping turn ideas into successful outcomes.
       <br><br>
       What excites me most is working at the intersection of technology and people. I enjoy leveraging my technical background while partnering with engineers, product teams, and stakeholders to align goals, solve complex problems, and turn ideas into reality. This combination of technical problem-solving, communication, and collaboration allows me to have the greatest impact and is the type of work I find most fulfilling.
    </p>
  </div>
</div>

<div class="dashed"></div>

## Education

<div class="about-entry">
  <div>
    <div class="about-entry-title">University of Illinois Urbana-Champaign</div>
    <div class="about-entry-sub">B.S. in Computer Science</div>
  </div>
  <div class="about-entry-date">2020 – 2023</div>
</div>

<div class="dashed"></div>

## Work Experience

<div class="about-entry">
  <div>
    <div class="about-entry-title">Job Title &middot; Company Name</div>
    <div class="about-entry-desc">Brief description of your role and what you worked on.</div>
  </div>
  <div class="about-entry-date">2024 – present</div>
</div>

<div class="about-entry">
  <div>
    <div class="about-entry-title">Job Title &middot; Company Name</div>
    <div class="about-entry-desc">Brief description of your role and what you worked on.</div>
  </div>
  <div class="about-entry-date">2023</div>
</div>

<div class="dashed"></div>

## Volunteering &amp; Activities

<div class="about-entry">
  <div>
    <div class="about-entry-title">Role &middot; Organization</div>
    <div class="about-entry-desc">Brief description of what you did or contributed.</div>
  </div>
  <div class="about-entry-date">2023 – present</div>
</div>

<div class="dashed"></div>

## Hobbies 
<div class="hobby-chips">
  <span 
    class="tag hobby-tag" 
    data-info="I grew up swimming competitivly and its still one of my favorite activitiers! I swim most days after work and am constantly trying to convince people to start swimming/find people who swim. My journey to find more people who swim lead me to joing SF Tsunami and now they are proudly my new swim group! My stroke is butterfly and Im currently working up towards swimming in the bay (scary and cold)." 
    data-photo="/assets/images/swim.png">Swimming
  </span>

  <span 
    class="tag hobby-tag" 
    data-info="I started making jewlery a few years ago- I missed having a ccrative hobby in my life and was tired of doom-scrolling my life away. I learned how to make a variety of jewlery but making earrings is my favorite. Over the years I've made a steady amount of earrings and most earrings I wear today are ones I made myself. I would like to put out a small collection someday, which is what inspired the BijourBreakdown project! " 
    data-photo="/assets/images/earring.png">Jewelry
  </span>

  <span 
    class="tag hobby-tag" 
    data-info="I recently started running and it's quickly becoming one of my favorite hobbies. I love long runs on Marina Green and down Lake Street. My most recent race is the San Francisco Alexi Pappas 10K. Slowly building up to longer milage!" 
    data-photo="/assets/images/run.png">Running
  </span>

  <span 
    class="tag hobby-tag" 
    data-info="I met a lot of my friends through volo and its always a positive in my week. I loved volo dodgebal and my friend group has recently started their own version of volo every week wwhere we play a different sport each week!." 
    data-photo="/assets/images/volo.jpg">Volo
  </span>

  <span 
    class="tag hobby-tag" 
    data-info="I have a beloved cat names Luna I adopted 2 years ago. She is the sweetest cat and loced by everyone who meets her. We spend lots of time playing with her mouse toys, going on outdoor adventures, and watching birds on our balcony. Luna is 8 years old and enjoys getting belly runs and is obsessed with any and all cat food, but is repulsed by literally all human food." 
    data-photo="/assets/images/luna2.JPG">Luna
  </span>

  <span 
    class="tag hobby-tag" 
    data-info="I love baking and recently bought a KitchainAid mixer. I bake almost every week and am constantly trying to offload the extra baked goods I have to my friends and roomatres. My favorite thing to make is Tiramisu and any pumpkin flavoried baked good." 
    data-photo="/assets/images/tiramisu.jpeg">Baking
  </span>
</div>

<div class="hobby-detail" id="hobby-detail">
  <img class="hobby-detail-photo" id="hobby-detail-photo" src="" alt="">
  <div class="hobby-detail-text" id="hobby-detail-text"></div>
</div>

<script>
(function () {
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
