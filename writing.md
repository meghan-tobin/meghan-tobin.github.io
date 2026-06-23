---
layout: about
title: Writing
---

<h1>Writing</h1>

<p>Technical writing, research notes, and essays. Links will go live as pieces are published.</p>

<ul class="writing-list">
  {% for item in site.data.home.writing_entries %}
    <li class="writing-item">
      {% if item.url %}
        <a href="{{ item.url }}" class="writing-item-title">{{ item.title }}</a>
      {% else %}
        <span class="writing-item-title writing-item-placeholder">{{ item.title }}</span>
      {% endif %}
      {% if item.desc %}
        <p class="writing-item-desc">{{ item.desc }}</p>
      {% endif %}
    </li>
  {% endfor %}
</ul>
