---
layout: default
title: About
---

<section class="hero">
  <p class="eyebrow">Data Portfolio — Log 001</p>
  <h1>Hi, I'm Amara.</h1>
  <h1>Welcome to my data showroom!</h1>
  <p class="hero__lede">
    I'm a data enthusiast who likes turning
    messy datasets into clear, usable insights. This site is a running
    log of the projects I've shipped along the way.
  </p>
</section>

<section class="bio">
  <p>
    [One or two short paragraphs about you: your background, what kind of
    problems you like working on, and what tools you reach for first. Keep
    it conversational — write like you're introducing yourself at a meetup,
    not like a resume header.]
  </p>
  <p>
    [Optional second paragraph: what you're currently learning, a domain
    you specialize in, or a fun fact that makes you memorable.]
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
