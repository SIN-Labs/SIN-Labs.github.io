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
    <div class="team-member">
        <a href="{{ person.url }}">
            <img src="{{ person.image }}" alt="{{ person.title }}" />
            <h3>{{ person.title }}</h3>
        </a>
        <p>{{ person.excerpt }}</p>
    </div>
    {% endfor %}
</div>

## Principal Investigators
<div class="team-grid">
    {% assign pis = site.team | where: "role", "pi" %}
    {% for person in pis %}
    <div class="team-member">
        <a href="{{ person.url }}">
            <img src="{{ person.image }}" alt="{{ person.title }}" />
            <h3>{{ person.title }}</h3>
        </a>
        <p>{{ person.excerpt }}</p>
    </div>
    {% endfor %}
</div>

## Students
<div class="team-grid">
    {% assign students = site.team | where: "role", "student" %}
    {% for person in students %}
    <div class="team-member">
        <a href="{{ person.url }}">
            <img src="{{ person.image }}" alt="{{ person.title }}" />
            <h3>{{ person.title }}</h3>
        </a>
        <p>{{ person.excerpt }}</p>
    </div>
    {% endfor %}
</div>

## Research Assistants
<div class="team-grid">
    {% assign assistants = site.team | where: "role", "research assistant" %}
    {% for person in assistants %}
    <div class="team-member">
        <a href="{{ person.url }}">
            <img src="{{ person.image }}" alt="{{ person.title }}" />
            <h3>{{ person.title }}</h3>
        </a>
        <p>{{ person.excerpt }}</p>
    </div>
    {% endfor %}
</div>