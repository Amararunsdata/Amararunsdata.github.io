---
layout: default
title: About
---

<section class="hero hero--with-photo">
  <img class="hero__photo" src="{{ '/assets/images/profile.jpg' | relative_url }}" alt="Photo of Amara">
  <div class="hero__text">
    <p class="eyebrow">Data Portfolio — Log 001</p>
    <h1>Hi, I'm Amara.</h1>
    <h1>Welcome to my data showroom!</h1>
    <p class="hero__lede">
      I'm a data enthusiast who likes turning
      messy datasets into clear, usable insights. This site is a running
      log of the projects I've shipped along the way.
    </p>
  </div>
</section>

<section class="bio">
  <p>
    I'm a Data Analytics professional with a background in market research,
    digital marketing, and business intelligence. I enjoy turning messy,
    real-world data into something structured, useful, and easy to
    understand — whether that means building a database, finding patterns
    in customer data, or creating a dashboard that actually answers a
    business question.
  </p>
  <p>
    These days, I'm particularly interested in designing data pipelines and
    using AI to automate data workflows.
  </p>
</section>

<section class="tools">
  <p class="tools__label">Tools I reach for</p>
  <ul class="tools__list">
    <li>Python</li>
    <li>pandas</li>
    <li>SQL</li>
    <li>scikit-learn</li>
    <li>Tableau</li>
    <li>matplotlib</li>
    <li>Jupyter</li>
  </ul>
</section>

<section class="record">
  <div class="record__row">
    <span class="record__key">email</span>
    <span class="record__value"><a href="mailto:{{ site.email }}">{{ site.email }}</a></span>
  </div>
  <div class="record__row">
    <span class="record__key">github</span>
    <span class="record__value"><a href="https://github.com/{{ site.github_username }}">github.com/{{ site.github_username }}</a></span>
  </div>
  <div class="record__row">
    <span class="record__key">linkedin</span>
    <span class="record__value"><a href="{{ site.linkedin_url }}">linkedin</a></span>
  </div>
</section>
