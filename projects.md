---
layout: page
title: Projects
---

{% for project in site.projects %}

## {{ project.title }}

![Project Image]({{ project.image }})

{{ project.description }}

{% if project.insights %}
**Key Insights:**
<ul>
{% for insight in project.insights %}
  <li>{{ insight }}</li>
{% endfor %}
</ul>
{% endif %}

[View Project]({{ project.github }})

---

{% endfor %}
