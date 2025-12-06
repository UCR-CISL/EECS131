---
layout: page
title: 2026 Winter
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

Lecture: Mon, Wen 12:30-13:50, HMNSS 1501

Lab: Tue 11:00-12:50 (Sec. 1), 13:00-14:50 (Sec. 2), WCH 128

<iframe style="width:100%; height:500px; overflow:hidden" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vSyp552S8DUshrwdMwsoaI7p5rIrqbxah6H864xKBkZyGrziRI_tV69F2T0z2p66w/pubhtml?gid=1225311029&amp;widget=false&amp;chrome=false&amp;gid=0&amp;range=A1:G21&amp;headers=false"></iframe> 



### Labs and Final Project
Students form into teams of two (2) to finish the labs and the final project using Jetson Nano, plus any compatible additional peripherals that the team can provide.

- Lab 1: Profiling your edge device
- Lab 2: Running ML on the edge
- Lab 3: Edge networking
- Lab 4: Cloud offloading
- Final Project: Design your favorite Edge ML application

### Selected Final Project Demos


