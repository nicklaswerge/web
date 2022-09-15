---
layout: page
permalink: /team/
title: team
description: Adaptive Intelligence Lab 
nav: true
# nav_order: 3
---

<article>
{% if site.data.team.leaders %}
    {% for person in site.data.team.leaders %}
        {% include team.html %}
    {% endfor %}
    ---
{% endif %}

{% if site.data.team.postdoctorals %}
    ## Postdoctoral Researchers
    {% for person in site.data.team.postdoctorals %}
        {% include team.html %}
    {% endfor %}
    ---
{% endif %}


{% if site.data.team.phds %}
    ## PhD Students
    {% for person in site.data.team.phds %}
        {% include team.html %}
    {% endfor %}
    ---
{% endif %}
<\article>