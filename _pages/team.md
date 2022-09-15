---
layout: page
permalink: /team/
title: team
description: Adaptive Intelligence Lab 
nav: true
# nav_order: 3
---
<header class="post-header">
    <h1 class="post-title">Adaptive Intelligence Lab </h1>
</header>

<div class="projects column">

  {% assign sorted= site.data.team.leaders | sort: "name" %}
  {% for member in sorted %}    

  <div class="card mb-3 hoverable card-horizontal">
    <div class="row no-gutters ">
      <div class="col-md-4">
        {% if member.img %}
        <img class="card-img" src="/assets/img/{{ member.img | relative_url }}" alt="{{ member.name }}">
        {% endif %}
      </div>
      <div class="col">
        <h2 class="card-title">{{ member.name }}</h2>
      </div>
    </div>
  </div>

{% endfor %}

</div>

---

<div class="projects column">

  {% assign sorted= site.data.team.phds | sort: "name" %}
  {% for member in sorted %}    

  <div class="card mb-3 hoverable card-horizontal">
    <div class="row no-gutters ">
      <div class="col-md-4">
        {% if member.img %}
        <img class="card-img" src="/assets/img/{{ member.img | relative_url }}" alt="{{ member.name }}">
        {% endif %}
      </div>
      <div class="col">
        <h2 class="card-title">{{ member.name }}</h2>
      </div>
    </div>
  </div>

{% endfor %}

</div>