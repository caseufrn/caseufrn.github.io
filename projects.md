---
layout: default
permalink: /projects
title: "Projects"
type:
  - "current"
  - "past"
---

## Projects


<!-- Incluir projetos no arquivo projects.csv, no diretório _data -->
{% include projectsection.html title="Current" type="current" data=site.data.projects %}

{% include projectsection.html title="Past" type="past" data=site.data.projects %}
