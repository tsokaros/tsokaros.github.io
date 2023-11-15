---
layout: page
permalink: /COCAL/
title: COCAL code
description: 
nav: false
nav_order: 4
---

### COCAL code

{% if site.data.repositories.COCAL %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.COCAL %}
    {% include repository/repo.html repository=repo %}
  {% endfor %}
</div>
{% endif %}