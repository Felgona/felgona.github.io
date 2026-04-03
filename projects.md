---
layout: page
title: Projects
---

<style>
.card {
  background: white;
  padding: 20px;
  border-radius: 12px;
  margin-bottom: 40px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.08);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 20px rgba(0,0,0,0.15);
}

.button {
  display:inline-block;
  margin-top:15px;
  padding:10px 18px;
  background-color:#007acc;
  color:white;
  text-decoration:none;
  border-radius:6px;
  font-weight:bold;
}
</style>

{% for project in site.projects %}

<div class="card">

  <h2>{{ project.title }}</h2>

  <img src="{{ project.image }}" style="width:100%; border-radius:10px;">

  <p>{{ project.description }}</p>

  {% if project.insights %}
  <strong>Key Insights:</strong>
  <ul>
    {% for insight in project.insights %}
      <li>{{ insight }}</li>
    {% endfor %}
  </ul>
  {% endif %}

  {% if project.impact %}
  <strong>Business Impact:</strong>
  <ul>
    {% for item in project.impact %}
      <li>{{ item }}</li>
    {% endfor %}
  </ul>
  {% endif %}

  <a href="{{ project.github }}" target="_blank" class="button">
    View Project
  </a>

</div>

{% endfor %}
