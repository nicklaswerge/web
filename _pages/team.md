---
layout: page
permalink: /team/
title: team
description: 
nav: true
# nav_order: 3
---
<header class="post-header">
    <h1 class="post-title">Adaptive Intelligence Lab </h1>
</header>

<div class="projects column">

  {% assign sorted= site.data.team.leaders | sort: "name" %}
  {% for member in sorted %}    
    {% include team.html name=member %}
  {% endfor %}

</div>

---

<div class="projects column">

  {% assign sorted= site.data.team.phds | sort: "name" %}
  {% for member in sorted %}        
    {% include team.html name=member %}
  {% endfor %}

</div>