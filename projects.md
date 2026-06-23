---
layout: about
title: Projects
---

<h1>Projects</h1>

<p>Four projects showcasing my work. Click any card to read the full overview.</p>

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
              <img src="{{ project.graphic }}" alt="{{ project.title }}">
            {% endif %}
          </div>
        </a>
      </li>
    {% endfor %}
  </ul>
</div>
