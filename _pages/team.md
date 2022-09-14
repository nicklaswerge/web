---
layout: page
permalink: /team/
title: team
description: Adaptive Intelligence Lab 
nav: true
# nav_order: 3
---


{% if site.data.team.leaders %}
    {% for person in site.data.team.leaders %}
        {{ person.name }}
            {% if person.mail %} "hey"
                {{ person.mail }}
            {% endif %}
            {% if person.webpage %}
                {{ person.webpage }}
            {% endif %}
            {% if person.scholar %}
                {{ person.scholar }}
            {% endif %}
    {% endfor %}
    ---
{% endif %}

{% if site.data.team.postdoctorals %}
    ## Postdoctoral Researchers
    {% for person in site.data.team.postdoctorals %}
        {{ person.name }}
            {% if person.mail %} "hey"
                {{ person.mail }}
            {% endif %}
            {% if person.webpage %}
                {{ person.webpage }}
            {% endif %}
            {% if person.scholar %}
                {{ person.scholar }}
            {% endif %}
    {% endfor %}
    ---
{% endif %}


{% if site.data.team.postdoctorals %}
    ## Postdoctoral Researchers
        {{ person.name }}
            {% if person.mail %} "hey"
                {{ person.mail }}
            {% endif %}
            {% if person.webpage %}
                {{ person.webpage }}
            {% endif %}
            {% if person.scholar %}
                {{ person.scholar }}
            {% endif %}
    {% endfor %}
    ---
{% endif %}