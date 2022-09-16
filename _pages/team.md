---
layout: page
permalink: /team/
title: team
description: 
nav: true
# nav_order: 3
---
<article>
<header class="post-header">
    <h1 class="post-title">Adaptive Intelligence Lab </h1>
</header>

{% if site.data.team.leaders %}
    <h2 id="principal-investigator">Principal Investigator</h2>
    <div class="projects column">
        {% assign sorted= site.data.team.leaders | sort: "name" %}
        {% for member in sorted %}
            {% include team.html member=member %}
        {% endfor %}
    </div>
{% endif %}


{% if site.data.team.postdoctorals %}
    <h2 id="postdoctoral-researchers">Postdoctoral Researchers</h2>
    <div class="projects column">
        {% assign sorted= site.data.team.postdoctorals | sort: "name" %}
        {% for member in sorted %}
            {% include team.html member=member %}
        {% endfor %}
    </div>
{% endif %}


{% if site.data.team.phds %}
    <h2 id="phd-students">PhD Students</h2>
    <div class="projects column">
        {% assign sorted= site.data.team.phds | sort: "name" %}
        {% for member in sorted %}
            {% include team.html member=member %}
        {% endfor %}
    </div>
{% endif %}


{% if site.data.team.mscs %}
    <h2 id="msc-students">MSc Students</h2>
    <div class="projects column">
        {% assign sorted= site.data.team.mscs | sort: "name" %}
        {% for member in sorted %}
            {% include team.html member=member %}
        {% endfor %}
    </div>
{% endif %}


{% if site.data.team.alumnis %}
    <h2 id="alumni">Alumni</h2>
    <div class="projects column">
        {% assign sorted= site.data.team.alumnis | sort: "name" %}
        {% for member in sorted %}
            {% include team.html member=member %}
        {% endfor %}
    </div>
{% endif %}


</article>
