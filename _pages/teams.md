---
layout: default
title: Our Team
hero_image: "/assets/images/team.jpg"
hero_title: Team
permalink: /team/
---

# Meet The Team

## Director
<div class="team-grid">
    {% assign directors = site.team | where: "role", "director" %}
    {% for person in directors %}
        {% include teambox.html %}
    {% endfor %}
</div>

## Principal Investigators
<div class="team-grid">
    {% assign pis = site.team | where: "role", "principal investigator" %}
    {% for person in pis %}
        {% include teambox.html %}
    {% endfor %}
</div>

## Students
<div class="team-grid">
    {% assign students = site.team | where: "role", "student" %}
    {% for person in students %}
        {% include teambox.html %}
    {% endfor %}
</div>

## Research Assistants
<div class="team-grid">
    {% assign assistants = site.team | where: "role", "research assistant" %}
    {% for person in assistants %}
        {% include teambox.html %}
    {% endfor %}
</div>