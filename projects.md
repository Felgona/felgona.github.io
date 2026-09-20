---
layout: page
title: Projects
---

<link rel="stylesheet" href="/assets/css/style.css">

{% for project in site.projects %}

<div class="card">

  <h2>{{ project.title }}</h2>

  <img src="{{ project.image }}" style="width:100%; border-radius:10px; margin-top:10px;">

  <p style="margin-top:15px; font-size:16px;">
    {{ project.description }}
  </p>

  <details style="margin-top:15px;">

    <summary style="cursor:pointer; font-weight:bold; color:#007acc;">
      Read more
    </summary>

    {% if project.insights %}
    <p><strong>Key Insights:</strong></p>
    <ul>
      {% for insight in project.insights %}
        <li>{{ insight }}</li>
      {% endfor %}
    </ul>
    {% endif %}

    {% if project.impact %}
    <p><strong>Business Impact:</strong></p>
    <ul>
      {% for item in project.impact %}
        <li>{{ item }}</li>
      {% endfor %}
    </ul>
    {% endif %}

    <a href="{{ project.github }}" target="_blank" class="button">
      View Project
    </a>

  </details>

</div>

<hr style="margin:40px 0;">

{% endfor %}
