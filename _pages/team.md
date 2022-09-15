---
layout: page
permalink: /team/
title: team
description: 
nav: true
leaders: site.data.team.leaders
phds: site.data.team.phds
# nav_order: 3
---
<header class="post-header">
    <h1 class="post-title">Adaptive Intelligence Lab </h1>
</header>

<div class="projects column">

  {% assign sorted= page.leaders | sort: "name" %}
  {% for member_i in sorted %}    
  {% assign member = member_i %}

  <div class="card hoverable">
    <div class="row no-gutters">
      <div class="col-sm-4 col-md-3">
        <img src="/sduadaptiveintelligencelab/assets/img/melih_kandemir.png" class="card-img img-fluid" alt="Leslie M. Cope, PhD">
      </div>
      <div class="team col-sm-8 col-md-9">
        <div class="card-body">
          <a href="https://www.google.com" target="_blank" rel="noopener noreferrer">
            <h5 class="card-title">{{ member_i.name }}</h5>       
            <p class="card-text">
              demodemo
            </p>
          </a>
          <a href="mailto:akgula15@itu.edu.tr" class="card-link"><i class="fas fa-envelope"></i></a> 
          <a href="https://www.google.com" class="card-link" target="_blank" rel="noopener noreferrer"><i class="fas fa-globe"></i></a>   
        </div>
      </div>
    </div>
  </div>
  <p> </p>



{% endfor %}

</div>

---

<div class="projects column">

  {% assign sorted= page.phds | sort: "name" %}
  {% for member_i in sorted %}    
  {% assign member = member_i %}

  <div class="card hoverable">
    <div class="row no-gutters">
      <div class="col-sm-4 col-md-3">
        <img src="/sduadaptiveintelligencelab/assets/img/melih_kandemir.png" class="card-img img-fluid" alt="Leslie M. Cope, PhD">
      </div>
      <div class="team col-sm-8 col-md-9">
        <div class="card-body">
          <a href="https://www.google.com" target="_blank" rel="noopener noreferrer">
            <h5 class="card-title">{{ member.name }}</h5>       
            <p class="card-text">
              demodemo
            </p>
          </a>
          <a href="mailto:akgula15@itu.edu.tr" class="card-link"><i class="fas fa-envelope"></i></a> 
          <a href="https://www.google.com" class="card-link" target="_blank" rel="noopener noreferrer"><i class="fas fa-globe"></i></a>   
        </div>
      </div>
    </div>
  </div>
  <p> </p>


{% endfor %}

</div>