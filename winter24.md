---
layout: page
title: Winter 2024
---

{% assign team = site.data.team_winter24 | sort : "name" %}

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

Lecture: Mon, Wen 9:30-10:50, Olmsted Hall 1212

Discussion: Wen 12:00-13:00 (Sec. 2), 13:00-14:00 (Sec. 1), WCH128

<iframe style="width:100%; height:600px; overflow:hidden" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vSndp1VlhR48elmZEjsBQVyZ0-egKxLLYYWanEz1kNsOMQfT3Tdr1IImkOmiMAgGqTsvEtVBj0ewGnG/pubhtml?widget=false&amp;chrome=false&amp;gid=0&amp;range=A1:G21&amp;headers=false"></iframe>

### Labs and Final Project
Students form into teams of two (2) to finish the labs and the final project using Jetson Nano, plus any compatible additional peripherals that the team can provide.

- Lab 1: Profiling your edge device
- Lab 2: Running ML on the edge
- Lab 3: Edge networking
- Lab 4: Cloud offloading
- Final Project: Design your favorite Edge ML application