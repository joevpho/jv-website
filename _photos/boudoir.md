---
layout: gallery
title: "Boudoir"
description: "A journey through my ink..."
image: "assets/images/featured-post/post-4.jpg"
permalink: /pictures/boudoir/
categories: 
  - "Writings"
tags:
  - "Writings"
  - "Kink"
  - "BDSM"
files:
  - path: "assets/images/featured-post/post-1.jpg"
  - path: "assets/images/featured-post/post-2.jpg"
  - path: "assets/images/featured-post/post-3.jpg"
  - path: "assets/images/featured-post/post-4.jpg"
  - path: "assets/images/featured-post/post-5.jpg"
  
---
<h2 class="mb-4">{{ page.title | escape }}</h2>

<section>
  <div class="container-fluid p-sm-0">
    <div class="row featured-post-slider">
        {% for img in page.files %}
        <div class="col-lg-3 col-sm-6 mb-2 mb-lg-0 px-1">
          <article class="card bg-dark text-center text-white border-0 rounded-0">
            <img class="card-img rounded-0 img-fluid w-100" src="{{img.path | relative_url}}" alt="{{cat.title}}">
<!--            {{img.path}}-->
  <!--          <div class="card-img-overlay">-->
  <!--            <div class="card-content">-->

  <!--            </div>-->
  <!--          </div>-->
          </article>
        </div>
        {% endfor %}
    </div>
  </div>
</section>