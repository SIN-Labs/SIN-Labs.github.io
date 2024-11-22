---
layout: default
title: "Meet the Team"
hero_image: "/assets/images/team.jpg"
hero_title: "Team"
permalink: /sin/
team_members:
  - name: "Hakwan Lau"
    role: "Director"
    image: "/assets/images/team/hakwan.png"
    url: "/team/hakwan-lau"
    description: "Director of the Perceptual Intelligence Lab, Hakwan focuses on cognitive neuroscience, neurofeedback, and perceptual studies."
    research_interest: "Cognitive Neuroscience, Neurofeedback, Perception"
---
<!-- Dynamic Content -->
<section class="team-section">
    <div class="row justify-content-center">
        {% for member in page.team_members %}
        <div class="col-md-6 col-lg-6 mb-30px">
            <a href="{{ site.baseurl }}{{ member.url }}" class="text-dark" style="text-decoration: none;">
                <div class="listfeaturedtag h-100 d-flex flex-wrap flex-lg-nowrap" 
                     style="border: 1px solid rgba(0, 0, 0, 0.125); border-radius: 0.25rem; padding: 20px;">
                    <!-- Image Section -->
                    <div class="featured-box-img-cover" 
                         style="background-image: url('{{ member.image }}'); 
                                background-size: cover; 
                                background-position: center; 
                                width: 100%; 
                                aspect-ratio: 3 / 4; 
                                border-radius: 0.25rem;">
                    </div>
                    <!-- Content Section -->
                    <div class="card-body text-left" style="width: 100%; padding-top: 20px;">
                        <h2 class="card-title" 
                            style="font-size: 1.5rem; font-weight: 700; line-height: 1.25; margin-top: 15px;">
                            {{ member.name }}
                        </h2>
                        <h4 class="card-text" 
                            style="color: rgba(0, 0, 0, .44); font-size: 0.95rem; line-height: 1.6; 
                                   font-weight: 400; margin-top: 15px;">
                            {{ member.role }}
                        </h4>
                        <h4 class="card-text" 
                            style="color: rgba(0, 0, 0, .44); font-size: 0.95rem; line-height: 1.6; 
                                   font-weight: 400; margin-top: 15px;">
                            {{ member.description }}
                        </h4>
                        <h4 class="card-text" 
                            style="color: rgba(0, 0, 0, .44); font-size: 0.95rem; line-height: 1.6; 
                                   font-weight: 400; margin-top: 15px;">
                            <strong>Research Interest:</strong> {{ member.research_interest }}
                        </h4>
                    </div>
                </div>
            </a>
        </div>
        {% endfor %}
    </div>
</section>
