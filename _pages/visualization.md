---
layout: page
permalink: /visualization/
title: Visualization
description: 
nav: false
nav_order: 4
---
## The Illinois Numerical Relativity Visualization Primer

{% if site.data.repositories.visualization %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for item in site.data.repositories.visualization %}
    {% if item.repository %}
      {% include repository/repo.html repository=item.repository image=item.image %}
    {% else %}
      {% include repository/repo.html repository=item %}
    {% endif %}
  {% endfor %}
</div>
{% endif %}

<br/>
<!--- ## Movies   --->


