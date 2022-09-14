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
    <!-- The paddingtop and margin-top edits allow anchors to link properly. -->
    <div id = "{{person.name | replace: ' ', '-'}}" class="row" style="padding-top: 60px; margin-top: -60px;">
        {% if person.image %}
        <img style="float: right; width: 42%; padding-left: 20px;" src="{{ person.image | prepend: '/assets/img/' | prepend: site.baseurl | prepend: site.url }}" alt="photo of {{person.name}}">
        {% endif %}
        <div>
            <h4>{{person.name}}{% if person.title %}, {{person.title}} {% endif %}</h4><br>
            {% if person.mail %}
                <a href="mailto:{{person.mail}}" class="cardlink"><i class="fa fa-envelope"></i></a> <br>
            {% endif %}
            {% if person.webpage %}
            <i class="fa fa-globe"></i> <a href= "{{person.webpage}}" target="_blank">{{person.webpage}}</a> <br>
            {% endif %}
            {% if person.scholar %}
            <i class="ai ai-google-scholar"></i> <a href= "{{person.scholar}}" target="_blank"> Scholar Citations </a> <br>
            {% endif %}
            {% if person.orcid %}
            <i class="ai ai-orcid"></i> <a href="http://{{person.orcid}}" target="_blank"> {{person.orcid}}</a> <br>
            {% endif %}
            {% if person.linkedin %}
            <a href= "{{person.linkedin}}" target="_blank"><i class="fab fa-linkedin"></i> </a> <br>
            {% endif %}
            {% if person.twitter %}
            <a href= "{{person.twitter}}" target="_blank"><i class="fab fa-twitter"></i> </a> <br>
            {% endif %}
            {% if person.instagram %}
            <a href= "{{person.instagram}}" target="_blank"><i class="fab fa-instagram"></i> </a> <br>
            {% endif %}
            

        </div>
        <div class="col-sm-8">
            <p class="text-justify">{{person.about | markdownify}}</p>
        </div>
    </div>
    <hr>
    {% endfor %}
    ---
{% endif %}

{% if site.data.team.postdoctorals %}
    ## Postdoctoral Researchers
    {% for person in site.data.team.postdoctorals %}
    <!-- The paddingtop and margin-top edits allow anchors to link properly. -->
    <div id = "{{person.name | replace: ' ', '-'}}" class="row" style="padding-top: 60px; margin-top: -60px;">
        {% if person.image %}
        <img style="float: right; width: 42%; padding-left: 20px;" src="{{ person.image | prepend: '/assets/img/' | prepend: site.baseurl | prepend: site.url }}" alt="photo of {{person.name}}">
        {% endif %}
        <div>
            <h4>{{person.name}}{% if person.title %}, {{person.title}} {% endif %}</h4><br>
            {% if person.mail %}
                <a href="mailto:{{person.mail}}" class="cardlink"><i class="fa fa-envelope"></i></a> <br>
            {% endif %}
            {% if person.webpage %}
            <i class="fa fa-globe"></i> <a href= "{{person.webpage}}" target="_blank">{{person.webpage}}</a> <br>
            {% endif %}
            {% if person.scholar %}
            <i class="ai ai-google-scholar"></i> <a href= "{{person.scholar}}" target="_blank"> Scholar Citations </a> <br>
            {% endif %}
            {% if person.orcid %}
            <i class="ai ai-orcid"></i> <a href="http://{{person.orcid}}" target="_blank"> {{person.orcid}}</a> <br>
            {% endif %}
            {% if person.linkedin %}
            <a href= "{{person.linkedin}}" target="_blank"><i class="fab fa-linkedin"></i> </a> <br>
            {% endif %}
            {% if person.twitter %}
            <a href= "{{person.twitter}}" target="_blank"><i class="fab fa-twitter"></i> </a> <br>
            {% endif %}
            {% if person.instagram %}
            <a href= "{{person.instagram}}" target="_blank"><i class="fab fa-instagram"></i> </a> <br>
            {% endif %}
            

        </div>
        <div class="col-sm-8">
            <p class="text-justify">{{person.about | markdownify}}</p>
        </div>
    </div>
    <hr>
    {% endfor %}
    ---
{% endif %}


{% if site.data.team.postdoctorals %}
    ## Postdoctoral Researchers
    {% for person in site.data.team.postdoctorals %}
    <!-- The paddingtop and margin-top edits allow anchors to link properly. -->
    <div id = "{{person.name | replace: ' ', '-'}}" class="row" style="padding-top: 60px; margin-top: -60px;">
        {% if person.image %}
        <img style="float: right; width: 42%; padding-left: 20px;" src="{{ person.image | prepend: '/assets/img/' | prepend: site.baseurl | prepend: site.url }}" alt="photo of {{person.name}}">
        {% endif %}
        <div>
            <h4>{{person.name}}{% if person.title %}, {{person.title}} {% endif %}</h4><br>
            {% if person.mail %}
                <a href="mailto:{{person.mail}}" class="cardlink"><i class="fa fa-envelope"></i></a> <br>
            {% endif %}
            {% if person.webpage %}
            <i class="fa fa-globe"></i> <a href= "{{person.webpage}}" target="_blank">{{person.webpage}}</a> <br>
            {% endif %}
            {% if person.scholar %}
            <i class="ai ai-google-scholar"></i> <a href= "{{person.scholar}}" target="_blank"> Scholar Citations </a> <br>
            {% endif %}
            {% if person.orcid %}
            <i class="ai ai-orcid"></i> <a href="http://{{person.orcid}}" target="_blank"> {{person.orcid}}</a> <br>
            {% endif %}
            {% if person.linkedin %}
            <a href= "{{person.linkedin}}" target="_blank"><i class="fab fa-linkedin"></i> </a> <br>
            {% endif %}
            {% if person.twitter %}
            <a href= "{{person.twitter}}" target="_blank"><i class="fab fa-twitter"></i> </a> <br>
            {% endif %}
            {% if person.instagram %}
            <a href= "{{person.instagram}}" target="_blank"><i class="fab fa-instagram"></i> </a> <br>
            {% endif %}
        </div>
        <div class="col-sm-8">
            <p class="text-justify">{{person.about | markdownify}}</p>
        </div>
    </div>
    <hr>
    {% endfor %}
    ---
{% endif %}