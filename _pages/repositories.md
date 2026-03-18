---
layout: page
permalink: /repositories/
title: repositories
description: GitHub repositories for 3D deep learning, CAD analysis, and manufacturability research.
nav: true
nav_order: 4
---

{% if site.data.repositories.github_repos %}

## GitHub repositories

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
