---
layout: page
title: Projects
permalink: /projects/
nav: true
nav_order: 3
---

<div class="post">
  <div class="section">
  <h2>Template</h2>
  <hr>
  <div class="stuff">
    <img src="../assets/img/1.jpg" alt="">
    <div class="info">
      <h3>Person</h3>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent at urna felis. 
        Vivamus efficitur felis nec tempus accumsan. Phasellus vehicula ac lectus ut pharetra. 
        Nunc dignissim laoreet gravida. Mauris semper.</p>
    </div>
  </div>
  <div class="stuff">
    <img src="" alt="">
    <div class="info">
      <h3>Person</h3>
      <p>Description.</p>
    </div>
  </div>
  </div>

  <div class="section">
  <h2>Template</h2>
  <hr>
  <div class="stuff">
    <img src="" alt="">
    <div class="info">
      <h3>Person</h3>
      <p>Description.</p>
    </div>
  </div>
  <div class="stuff">
    <img src="" alt="">
    <div class="info">
      <h3>Person</h3>
      <p>Description.</p>
    </div>
  </div>
  </div>
</div>





<!--
---
layout: page
title: Projects and Interests
permalink: /projects/
description: 
nav: true
nav_order: 3
display_categories: [Research, Fun]
horizontal: false
---

comment* pages/projects.md 
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  comment* Display categorized projects
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
  comment* Generate cards for each project 
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

comment* Display projects without categories

{% assign sorted_projects = site.projects | sort: "importance" %}

  comment* Generate cards for each project

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
-->
