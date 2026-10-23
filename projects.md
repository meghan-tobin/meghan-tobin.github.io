---
layout: about
title: Projects
---

<h1>Projects</h1>

{% assign sorted_projects = site.projects | sort: 'order' %}
<div class="project-cards">
  <ul class="horizontal-list">
    {% for project in sorted_projects %}
      <li class="card">
        <a href="{{ project.url }}">
          <span class="header">{{ project.title }}</span>
          <hr />
          <div class="card-graphic">
            {% if project.graphic %}
              <img src="{{ project.graphic }}" alt="{{ project.title }}"{% if project.graphic_dark %} class="graphic-light"{% endif %}>
              {% if project.graphic_dark %}
                <img src="{{ project.graphic_dark }}" alt="{{ project.title }}" class="graphic-dark">
              {% endif %}
            {% endif %}
          </div>
        </a>
      </li>
    {% endfor %}
  </ul>
</div>
