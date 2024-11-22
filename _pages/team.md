---
layout: default
title: "Meet the Team"
hero_image: "/assets/images/team.jpg"
hero_title: "Team"
permalink: /sin/
team:
  - role: "Director"
    members:
      - name: "Hakwan Lau"
        image: "/assets/images/team/hakwan.png"
        excerpt: "Director of the Perceptual Intelligence Lab, Hakwan focuses on cognitive neuroscience, neurofeedback, and perceptual studies."
        research_interest: "Cognitive Neuroscience, Neurofeedback"
        link: "https://twitter.com/hakwanlau"
---
<!-- Dynamic Content -->
{% for group in page.team %}
<section class="team-section">
    <div class="section-title">
        <h2><span>{{ group.role }}</span></h2>
    </div>
    <div class="row justify-content-center">
        {% for person in group.members %}
        <div class="col-12 col-md-12 col-lg-6 mb-30px">
            <div class="listfeaturedtag h-100 d-flex flex-column flex-lg-row" style="border: 1px solid rgba(0, 0, 0, 0.125); border-radius: 0.25rem; padding: 20px;">
                <!-- Image Section -->
                <div class="featured-box-img-cover" style="background-image: url('{{ person.image }}'); background-size: cover; background-position: center; aspect-ratio: 3 / 4; border-radius: 0.25rem; width: 100%; height: 200px;" 
                     class="flex-shrink-0">
                </div>
                <!-- Content Section -->
                <div class="card-body text-left" style="padding: 15px; width: 100%;">
                    <h2 class="card-title" style="font-size: 1.3rem; font-weight: 700; line-height: 1.25; margin-top: 15px;">
                        {{ person.name }}
                    </h2>
                    <h4 class="card-text" style="color: rgba(0, 0, 0, .44); font-size: 0.95rem; line-height: 1.6; font-weight: 400; margin-top: 15px;">
                        {{ person.excerpt }}
                    </h4>
                    {% if person.research_interest %}
                    <h4 class="card-text" style="color: rgba(0, 0, 0, .44); font-size: 0.95rem; line-height: 1.6; font-weight: 400; margin-top: 15px;">
                        <strong>Research Interest:</strong> {{ person.research_interest }}
                    </h4>
                    {% endif %}
                    {% if person.link %}
                    <div class="mt-3">
                        <a href="{{ person.link }}" target="_blank">
                            <i class="fab fa-twitter"></i>
                        </a>
                    </div>
                    {% endif %}
                </div>
            </div>
        </div>
        {% endfor %}
    </div>
</section>
{% endfor %}