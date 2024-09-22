---
layout: default
title: "Meet the Team"
hero_iamge: "/assets/images/team.jpg"
hero_title: "Team"
permalink: /team/
---

<!-- Director Section -->
<section class="team-section">
    <div class="section-title">
        <h2><span>Director</span></h2>
    </div>
    <div class="row">
        <!-- Hardcoded Director Section -->
        <div class="col-md-6 col-lg-4 mb-30px">
            <div class="team-card h-100">
                <div class="team-image">
                    <img class="img-fluid" src="/assets/images/team/hakwan.jpg" alt="Hakwan Lau">
                </div>
                <div class="team-body">
                    <h3 class="team-title">Hakwan Lau</h3>
                    <p class="team-excerpt">Director of the Perceptual Intelligence Lab, Hakwan focuses on cognitive neuroscience, neurofeedback, and perceptual studies.</p>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- Principal Investigators Section -->
<section class="team-section">
    <div class="section-title">
        <h2><span>Principal Investigators</span></h2>
    </div>
    <div class="row">
        {% assign pis = site.team | where: "role", "principal investigator" %}
        {% for member in pis %}
            {% include teammember.html %}
        {% endfor %}
    </div>
</section>

<!-- Students Section -->
<section class="team-section">
    <div class="section-title">
        <h2><span>Students</span></h2>
    </div>
    <div class="row">
        {% assign students = site.team | where: "role", "student" %}
        {% for member in students %}
            {% include teammember.html %}
        {% endfor %}
    </div>
</section>

<!-- Research Assistants Section -->
<section class="team-section">
    <div class="section-title">
        <h2><span>Research Assistants</span></h2>
    </div>
    <div class="row">
        {% assign research_assistants = site.team | where: "role", "research assistant" %}
        {% for member in research_assistants %}
            {% include teammember.html %}
        {% endfor %}
    </div>
</section>