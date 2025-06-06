---
layout: page
title: "Projects"
permalink: /projects/
---

Here are some of the projects I’ve worked on:

{% for project in site.data.projects %}
---

### {{ project.title }}
**{{ project.subtitle }}**

{% for line in project.description %}
- {{ line }}
{% endfor %}

[GitHub Repo]({{ project.github }})  
[Live Site]({{ project.live_site }})

{% endfor %}
