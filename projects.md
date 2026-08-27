---
layout: default
title: Projects
permalink: /projects/
---

<section class="hero">
  <p class="eyebrow">Project Log</p>
  <h1>Projects</h1>
  <p class="hero__lede">
    A running log of things I've built and analyzed, newest first.
  </p>
</section>

<section class="log">
  {% for project in site.data.projects %}
  <article class="log-entry">
    <div class="log-entry__index">{{ forloop.index | prepend: "000" | slice: -3, 3 }}</div>
    <div class="log-entry__body">
      <h2 class="log-entry__title">
        {% if project.demo_url and project.demo_url != "" %}
          <a href="{{ project.demo_url }}">{{ project.title }}</a>
        {% elsif project.repo_url and project.repo_url != "" %}
          <a href="{{ project.repo_url }}">{{ project.title }}</a>
        {% else %}
          {{ project.title }}
        {% endif %}
      </h2>
      <p class="log-entry__desc">{{ project.description }}</p>
      {% if project.metrics %}
        <div class="log-entry__meta">{{ project.metrics }}</div>
      {% endif %}
      {% if project.tags %}
        <div class="log-entry__tags">
          {% for tag in project.tags %}<span>{{ tag }}</span>{% endfor %}
        </div>
      {% endif %}
      <div class="log-entry__links">
        {% if project.repo_url and project.repo_url != "" %}
          <a href="{{ project.repo_url }}">repo →</a>
        {% endif %}
        {% if project.demo_url and project.demo_url != "" %}
          <a href="{{ project.demo_url }}">demo →</a>
        {% endif %}
      </div>
    </div>
  </article>
  {% endfor %}
</section>
