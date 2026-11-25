---
layout: about
title: about
permalink: /
subtitle: Research Associate · Federal Reserve Bank of Boston

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p><a href='mailto:jackfterry20@gmail.com'>jackfterry20@gmail.com</a></p>
    <p><a href='/assets/pdf/cv.pdf'>Curriculum Vitae (PDF)</a></p>

selected_papers: false # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: false

latest_posts:
  enabled: false
---

<p class="jt-lede">I'm a Research Associate at the <a href="https://www.bostonfed.org">Federal Reserve Bank of Boston</a>, where I work on household decision making, labor, and health economics. I'm applying to PhD programs in economics.</p>

I took a slightly unusual route here. I started in medical physics with the <a href="https://bertoletlab.mgh.harvard.edu/">Bertolet Lab</a> at Massachusetts General Hospital, modeling radiation dose distributions in tumor treatment, before moving into economics, with an MSc thesis at the London School of Economics on the 1933 U.S. banking crisis. These days most of my research asks how recessions show up in people's lives: in births, in deaths, and in the welfare cost of the business cycle. You can find that work under [projects](/projects/).

{% assign latest = site.data.readings | sort: 'read', 'first' | last %}
{% if latest %}

<h2 class="jt-section-label">Recently read</h2>
<div class="jt-now">
  <p><a href="{{ latest.link }}">{{ latest.title }}</a></p>
  <p class="jt-now-meta">{{ latest.authors }} · {{ latest.read | append: '-01' | date: '%B %Y' }} · <a href="/reading/">full reading log →</a></p>
</div>
{% endif %}

<h2 class="jt-section-label">Outside of econ</h2>
<div class="jt-offhours">
  <button type="button" class="jt-flip" aria-pressed="false" aria-label="Running: show photo">
    <span class="jt-flip-inner">
      <span class="jt-flip-face jt-flip-front">
        <i class="fa-solid fa-person-running jt-offhours-icon" aria-hidden="true"></i>
        <span class="jt-flip-title">Running</span>
        <span class="jt-flip-text">Training to qualify for the Boston Marathon, chasing a BQ this spring.</span>
        <span class="jt-flip-hint"><i class="fa-solid fa-camera" aria-hidden="true"></i> see the photo</span>
      </span>
      <span class="jt-flip-face jt-flip-back">
        <img src="/assets/img/outside/running.jpg" alt="Jack holding a first-place plaque with a finisher's medal after the Lake Martin 27-mile race" loading="lazy" width="640" height="800">
        <span class="jt-flip-caption">Lake Martin Ultra – 27-mile winner</span>
      </span>
    </span>
  </button>
  <button type="button" class="jt-flip" aria-pressed="false" aria-label="Making music: show photo">
    <span class="jt-flip-inner">
      <span class="jt-flip-face jt-flip-front">
        <i class="fa-solid fa-music jt-offhours-icon" aria-hidden="true"></i>
        <span class="jt-flip-title">Making music</span>
        <span class="jt-flip-text">Writing and playing music.</span>
        <span class="jt-flip-hint"><i class="fa-solid fa-camera" aria-hidden="true"></i> see the photo</span>
      </span>
      <span class="jt-flip-face jt-flip-back">
        <img src="/assets/img/outside/music.jpg" alt="Jack playing bass guitar at a rooftop concert at sunset in Auburn, Alabama" loading="lazy" width="640" height="800">
        <span class="jt-flip-caption">Performing at a rooftop concert – Auburn, AL</span>
      </span>
    </span>
  </button>
  <button type="button" class="jt-flip" aria-pressed="false" aria-label="Sports: show photo">
    <span class="jt-flip-inner">
      <span class="jt-flip-face jt-flip-front">
        <i class="fa-solid fa-football jt-offhours-icon" aria-hidden="true"></i>
        <span class="jt-flip-title">Sports</span>
        <span class="jt-flip-text">A fan of everything from football to cycling.</span>
        <span class="jt-flip-hint"><i class="fa-solid fa-camera" aria-hidden="true"></i> see the photo</span>
      </span>
      <span class="jt-flip-face jt-flip-back">
        <img src="/assets/img/outside/sports.jpg" alt="Jack with two friends in the stands at Tottenham Hotspur Stadium after a match" loading="lazy" width="640" height="800">
        <span class="jt-flip-caption">Tottenham Hotspur Stadium</span>
      </span>
    </span>
  </button>
</div>

<script>
  document.querySelectorAll(".jt-flip").forEach(function (card) {
    card.addEventListener("click", function () {
      var flipped = card.classList.toggle("is-flipped");
      card.setAttribute("aria-pressed", flipped ? "true" : "false");
    });
  });
</script>

<p class="jt-disclaimer"><em>Views expressed here are my own and do not represent those of the Federal Reserve Bank of Boston or the Federal Reserve System.</em></p>
