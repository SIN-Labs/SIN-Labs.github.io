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
        {% assign directors = site.team | where: "position", "Director" %}
        {% for item in directors %}
            {% include teambox.html item=item %}
        {% endfor %}
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

<!-- Students
================================================== -->
<section class="team-section">
    <div class="section-title">
        <h2><span>Students</span></h2>
    </div>
    <div class="row justify-content-center">
        <div class="col-md-4 text-center">
            <img src="/assets/images/team/olga.jpg" alt="Olga Gulka" class="img-fluid" style="width: 300px; height: 400px; object-fit: cover;">
            <h3>Olga Gulka</h3>
            <p>Olga Gulka will be starting her PhD program in March 2025. Her research will focus on perception and neurofeedback in cognitive neuroscience.</p>
        </div>
    </div>
</section>

<!-- Research Assistants
================================================== -->
<section class="team-section">
    <div class="section-title">
        <h2><span>Research Assistants</span></h2>
    </div>
    <div class="row justify-content-center">
        <div class="col-md-4 text-center">
            <img src="/assets/images/team/junseo.jpeg" alt="Jun Seo Hwang" class="img-fluid" style="width: 300px; height: 400px; object-fit: cover;">
            <h3>Jun Seo Hwang</h3>
            <p>Jun Seo Hwang is a dedicated Research Assistant contributing to the Perceptual Intelligence Lab's neurofeedback and behavioral experiments.</p>
        </div>
    </div>
</section>