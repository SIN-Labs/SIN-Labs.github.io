---
layout: default
title: "Blog"
hero_image: "/assets/images/blog.jpg"
hero_title: "Blog"
pagination: 
  enabled: true
  collection: posts
permalink: /blog/
---

<!-- Blog Section
================================================== -->
<section class="blog-section">
    <div class="section-title">
        <h2><span><a href="{{ site.baseurl }}/blog" style="color: inherit; text-decoration: none;">Blog</a></span></h2>
    </div>
    <div class="row">
        {% assign sorted_posts = site.posts | sort: 'date' | reverse %}
        {% for post in sorted_posts %}
            {% include postbox.html %}
        {% endfor %}
    </div>
</section>

<!-- Pagination -->
<div class="bottompagination">
    <div class="pointerup"><i class="fa fa-caret-up"></i></div>
    <span class="navigation" role="navigation">
        {% include pagination.html %}
    </span>
</div>