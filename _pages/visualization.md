---
layout: page
permalink: /visualization/
title: Visualization
description: 
nav: false
nav_order: 4
---

<br>
## The Illinois Numerical Relativity Visualization Primer

<!-- Featured Image -->
{% if site.data.repositories.visualization_featured %}
{% for item in site.data.repositories.visualization_featured %}
<div class="featured-repo text-center mb-4" style="width: 90%; margin: 0 auto;">
  <a href="{{ item.repository }}" target="_blank">
    <img class="img-fluid" src="{{ item.image }}" alt="Featured Visualization" style="width: 100%;">
  </a>
</div>
{% endfor %}
{% endif %}

<br>
## The Abid Bot

{% if site.data.repositories.visualization %}
  <div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">

    {% for item in site.data.repositories.visualization %}
      {% if item contains 'abid_bot' %}
        <!-- Center abid_bot -->
        <div class="w-100 text-center my-3">
          {% include repository/repo.html repository=item %}
        </div>
      {% else %}
        <!-- Regular repos -->
        {% if item.repository %}
          {% include repository/repo.html repository=item.repository image=item.image %}
        {% else %}
          {% include repository/repo.html repository=item %}
        {% endif %}
      {% endif %}
    {% endfor %}

  </div>
{% endif %}


<br/>
<!--- ## Movies   --->


