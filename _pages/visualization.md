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


<!---  ### [The Illinois Numerical Relativity Visualization Primer](https://sjammi2.github.io/VisualizationGuideDocumentationTest/)  --->
### The Illinois Numerical Relativity Visualization Primer

{% if site.data.repositories.visualization_featured %}
{% for item in site.data.repositories.visualization_featured %}
<div class="featured-repo text-left mb-4" style="width: 90%; margin: 20 auto;">
  <a href="{{ item.repository }}" target="_blank">
    <img class="img-fluid" src="{{ item.image }}" alt="Featured Visualization" style="width: 100%;">
  </a>
</div>
{% endfor %}
{% endif %}

<br>
### [The Abid Bot](https://github.com/Illinois-Relativity-Group/abid_bot/)

{% if site.data.repositories.visualization_abid %}
{% for item in site.data.repositories.visualization_abid %}
<div class="featured-repo text-left mb-4" style="width: 50%; margin: 20 auto;">
  <a href="{{ item.repository }}" target="_blank">
    <img class="img-fluid" src="{{ item.image }}"  style="width: 50%;">
  </a>
</div>
{% endfor %}
{% endif %}



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


