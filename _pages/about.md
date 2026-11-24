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

<ul class="jt-interests">
  <li>labor</li>
  <li>health</li>
  <li>household decisions</li>
  <li>business cycles</li>
  <li>economic history</li>
</ul>

I took a slightly unusual route here. I started in medical physics, modeling radiation dose distributions in tumor treatment, before moving into economics, with an MSc thesis at the London School of Economics on the 1933 U.S. banking crisis. These days most of my research asks how recessions show up in people's lives: in births, in deaths, and in the welfare cost of the business cycle. You can find that work under [projects](/projects/).

{% assign latest = site.data.readings | sort: 'read' | last %}
{% if latest %}

<h2 class="jt-section-label">Recently read</h2>
<div class="jt-now">
  <p><a href="{{ latest.link }}">{{ latest.title }}</a></p>
  <p class="jt-now-meta">{{ latest.authors }} · {{ latest.read | append: '-01' | date: '%B %Y' }} · <a href="/reading/">full reading log →</a></p>
</div>
{% endif %}

<h2 class="jt-section-label">Off the clock</h2>
<div class="jt-offhours">
  <div class="jt-offhours-card">
    <i class="fa-solid fa-person-running jt-offhours-icon" aria-hidden="true"></i>
    <h4>Running</h4>
    <p>Out for a run whenever I can.</p>
  </div>
  <div class="jt-offhours-card">
    <i class="fa-solid fa-music jt-offhours-icon" aria-hidden="true"></i>
    <h4>Making music</h4>
    <p>Writing and playing music.</p>
  </div>
  <div class="jt-offhours-card">
    <i class="fa-solid fa-basketball jt-offhours-icon" aria-hidden="true"></i>
    <h4>Sports</h4>
    <p>Usually have a game on.</p>
  </div>
</div>

<p class="jt-disclaimer"><em>Views expressed here are my own and do not represent those of the Federal Reserve Bank of Boston or the Federal Reserve System.</em></p>
