---
layout: page
title: Projects
---

{% for project in site.projects %}

## {{ project.title }}

![Project Image]({{ project.image }})

{{ project.description }}

[View Project]({{ project.github }})

---

{% endfor %}
