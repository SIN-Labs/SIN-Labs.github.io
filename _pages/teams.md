---
layout: default
title: "Meet the Team"
hero_image: "/assets/images/team.jpg"
hero_title: "Team"
permalink: /team/
---

<!-- Director Section -->
<section class="team-section">
    <div class="section-title">
        <h2><span>Director</span></h2>
    </div>
    <div class="row justify-content-center">
        <!-- Hardcoded Director Section -->
        <div class="col-md-6 col-lg-4 mb-30px">
            <div class="team-card text-center  h-100">
                <div class="team-image">
                    <img class="img-fluid" src="/assets/images/team/hakwan.jpg" alt="Hakwan Lau" style="width: 80%; height: 400px; object-fit: cover;">
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
    <div class="row justify-content-center">
        <!-- Kayuet Liu -->
        <div class="col-md-6 col-lg-4 mb-30px">
            <div class="team-card text-center h-100">
                <div class="team-image">
                    <img class="img-fluid" src="/assets/images/team/kayuet.jpg" alt="Kayeut Liu" style="width: 80%; height: 400px; object-fit: cover;">
                </div>
                <div class="team-body">
                    <h3 class="team-title">Kayeut Liu</h3>
                    <p class="team-excerpt">Kayeut's group focuses on mental health conditions like depression and anxiety disorders, and their link to aphantasia, using large cohort data analysis.</p>
                </div>
            </div>
        </div>

        <!-- Ali Moharramipour -->
        <div class="col-md-6 col-lg-4 mb-30px">
            <div class="team-card text-center h-100">
                <div class="team-image">
                    <img class="img-fluid" src="/assets/images/team/ali.jpg" alt="Ali Moharramipour" style="width: 80%; height: 400px; object-fit: cover;">
                </div>
                <div class="team-body">
                    <h3 class="team-title">Ali Moharramipour</h3>
                    <p class="team-excerpt">Ali's group focuses on understanding the multidimensional nature of perception and uses human neuroimaging and mouse neurophysiological methods to study perceptual mechanisms.</p>
                </div>
            </div>
        </div>

        <!-- Qi Lin -->
        <div class="col-md-6 col-lg-4 mb-30px">
            <div class="team-card text-center h-100">
                <div class="team-image">
                    <img class="img-fluid" src="/assets/images/team/qi.jpg" alt="Qi Lin" style="width: 80%; height: 400px; object-fit: cover;">
                </div>
                <div class="team-body">
                    <h3 class="team-title">Qi Lin</h3>
                    <p class="team-excerpt">Qi's group focuses on individual differences in both perception and memory. She uses human neuroimaging and primate data to explore neural coding of images.</p>
                </div>
            </div>
        </div>
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