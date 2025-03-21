---
layout: page
title: Winter 2025
---

{% assign team = site.data.team_winter25 | sort : "name" %}

### Instructors

<div class="clearfix">
{% for people in team %} 
    {% if people.type == "PI" %} 
        {% include avatar_entry.html %} 
    {% endif %} 
{% endfor %}
</div>

### Teaching Assistants
<div class="clearfix">
{% for people in team %} 
    {% if people.type == "TA" %} 
        {% include avatar_entry.html %} 
    {% endif %} 
{% endfor %}
</div>

### Course Schedule

Lecture: Mon, Wen 9:30-10:50, WCH 143

Lab: Tue 11:00-12:50 (Sec. 1), 13:00-14:50 (Sec. 2), WCH 128

<iframe style="width:100%; height:600px; overflow:hidden" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vS1ZmsFhnrh07N_RcfPwi-HdG8lVb6RzJaOlbYmIBtIncRIjSqS9y99Mg9RZ7JQ1oBtyNag_3CVrMx8/pubhtml?widget=false&amp;chrome=false&amp;gid=0&amp;range=A1:G21&amp;headers=false"></iframe>

### Labs and Final Project
Students form into teams of two (2) to finish the labs and the final project using Jetson Nano, plus any compatible additional peripherals that the team can provide.

- Lab 1: Profiling your edge device
- Lab 2: Running ML on the edge
- Lab 3: Edge networking
- Lab 4: Cloud offloading
- Final Project: Design your favorite Edge ML application

### Selected Final Project Demos


<!-- * **Tesla Bot** We propose a general framework deployed through a NVIDIA Jetbot that can be
controlled by instructions generated by either a cloud or local LLM. These instructions are
generated based on the users query and a live image from the Jetbot. All the LLMs we
used were multimodal and would output general instructions that would be parsed into
specific function calls such as forward, left, and right with a estimated distance/degree.



<div class="video-container">
    <video muted autoplay loop width="100%">
        <source src="{{ site.baseurl }}/assets/videos/jerryli_CS131_Final_Project.mp4" type="video/mp4">
    </video>
</div> -->

{% assign project = site.data.team_winter25_project | sort : "name" %}

<!-- <div class="project-gallery">
    <div class="project-item">
        <h3>Tesla Bot</h3>
        <video muted autoplay loop controls>
            <source src="{{ site.baseurl }}/assets/videos/jerryli_CS131_Final_Project.mp4" type="video/mp4">
        </video>
    </div>

    <div class="project-item">
        <h3>American Sign Language (ASL) Detector</h3>
        <video muted autoplay loop controls>
            <source src="{{ site.baseurl }}/assets/videos/anisha_CS131_Final_Project.mp4" type="video/mp4">
        </video>
    </div>


</div> -->


<div class="clearfix">
<br>
{% for p in project %}
    <div class="videos">
        {% if p.web %}
            <h3><a href="{{ p.web }}" target="_blank">{{ p.name }}</a></h3> 
        {% else %}
            <h3>{{ p.name }}</h3> 
        {% endif %}
        <video width="640" height="360" controls>
        <source src="{{ site.baseurl }}/assets/videos/{{p.video}}" type="video/mp4">
        </video>
    </div>
{% endfor %}
</div>


