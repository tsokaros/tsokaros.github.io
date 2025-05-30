---
layout: page
title: Movies
permalink: /movies/
description: 
nav: false
nav_order: 2
display_categories: [2025, 2024, 2023, 2022, 2021, 2020, 2019, 2018] 
horizontal: true
---



<!-- pages/projects.md -->
<div class="projects">
<style>
  .category-header {
    color: var(--global-divider-color);
    border-bottom: 1px solid var(--global-divider-color);
    padding-top: 0.5rem;
    margin-top: 0rem;
    margin-bottom: 1rem;
    text-align: left;
  }
</style>

{%- if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {%- for category in page.display_categories %}
  <h2 class="category-header">{{ category }}</h2>
  {%- assign categorized_projects = site.projects | where: "category", category -%}
  {%- assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
    <div class="container">
        <div class="row">
        {%- for project in sorted_projects -%}
            <div class="col-xl-12">
                {% include projects_horizontal_temp3.html %}
            </div>
        {%- endfor %}
        </div>
    </div>
  {%- else -%}
    <div class="container">
        <div class="row">
        {%- for project in sorted_projects -%}
            <div class="col-xl-8">
                {% include projects_horizontal.html %}
            </div>
        {%- endfor %}
        </div>
    </div>
  {%- endif -%}
  {% endfor %}

{%- else -%}
<!-- Display projects without categories -->
  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
    <div class="container">
        <div class="row">
        {%- for project in sorted_projects -%}
            <div class="col-xl-12">
                {% include projects_horizontal_temp3.html %}
            </div>
        {%- endfor %}
        </div>
    </div>
  {%- else -%}
    <div class="container">
        <div class="row">
        {%- for project in sorted_projects -%}
            <div class="col-xl-8">
                {% include projects_horizontal.html %}
            </div>
        {%- endfor %}
        </div>
    </div>
  {%- endif -%}
{%- endif -%}
</div>
