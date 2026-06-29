---
layout: page
title: Projects
permalink: /projects/
description:
nav: true
nav_order: 4
display_categories:
horizontal: false
---

<!-- pages/projects.md -->
<div class="projects">
  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
</div>
