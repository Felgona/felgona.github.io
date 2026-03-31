---
layout: page
title: Projects
---

{% for project in site.projects %}

<div style="margin-bottom:50px;">

  <h2>{{ project.title }}</h2>

  <img src="{{ project.image }}" style="width:100%; border-radius:10px; margin-top:10px;">

  <p style="margin-top:15px; font-size:16px;">
    {{ project.description }}
  </p>

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

  <a href="{{ project.github }}" target="_blank" style="
    display:inline-block;
    margin-top:15px;
    padding:10px 18px;
    background-color:#007acc;
    color:white;
    text-decoration:none;
    border-radius:6px;
    font-weight:bold;
  ">
    View Project
  </a>

</div>

<hr style="margin:40px 0;">

{% endfor %}
