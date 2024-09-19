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
        {% include teammember.html %}
    {% endfor %}
</div>

## Principal Investigators
<div class="team-grid">
    {% assign pis = site.team | where: "role", "principal investigator" %}
    {% for person in pis %}
        {% include teammember.html %}
    {% endfor %}
</div>

## Students
<div class="team-grid">
    {% assign students = site.team | where: "role", "student" %}
    {% for person in students %}
        {% include teammember.html %}
    {% endfor %}
</div>

<!-- Posts Index
================================================== -->
<section class="recent-posts">
    <div class="section-title">
        <h2><span>Research Assistants</span></h2>
    </div>
    <div class="row listrecent">

        {% for post in paginator.posts %}
            {% include postbox.html %}
        {% endfor %}

    </div>
</section>