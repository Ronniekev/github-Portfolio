---
layout: single
title: "Projects"
permalink: /projects/
---

Here are some of the projects I’ve worked on:

{% for project in site.data.projects %}
---
### {{ project.title }}
**{{ project.subtitle }}**

<ul>
  {% for line in project.description %}
    <li>{{ line }}</li>
  {% endfor %}
</ul>

[GitHub Repo]({{ project.github }})  
{% if project.live_site %}
[Live Site]({{ project.live_site }})
{% endif %}

{% endfor %}
