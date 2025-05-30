---
layout: page
permalink: /visualization/
title: Visualization
description: 
nav: false
nav_order: 4
---

<!---
<div style="text-align:center;">
<font size="6">
<span style="color: red;">The Illinois Numerical Relativity Visualization Primer</span>
</font>
</div>     --->

<!---  [<font size="6">
The Illinois Numerical Relativity Visualization Primer
</font>](https://sjammi2.github.io/VisualizationGuideDocumentationTest/)   --->


{% assign all_repos = site.data.repositories.repositories %}

{% for item in all_repos %}
<div class="featured-repo text-left mb-4" style="width: 90%; margin: 20px auto;">
  <h3 style="margin-bottom: 10px;"><a href="{{ item.repository }}" target="_blank">{{ item.title }}</a></h3>
  {% if item.image %}
  <a href="{{ item.repository }}" target="_blank">
    <img src="{{ item.image }}" alt="{{ item.title }}"
     style="max-width: 90%; height: auto;">
  </a>
  {% endif %}
</div>
{% endfor %}



<!---
{% if site.data.repositories.visualization %}
  <div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
    {% for item in site.data.repositories.visualization %}
      {% if item contains 'abid_bot' %}
        <div class="w-100 text-center my-3">
          {% include repository/repo.html repository=item %}
        </div>
      {% else %}
        {% if item.repository %}
          {% include repository/repo.html repository=item.repository image=item.image %}
        {% else %}
          {% include repository/repo.html repository=item %}
        {% endif %}
      {% endif %}
    {% endfor %}
  </div>
{% endif %}
--->

<br/>
<!--- ## Movies   --->


