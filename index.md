---
title: "VisualAI Portfolio"
layout: splash
permalink: /
header:
  overlay_color: "#4BA9C8"
  overlay_filter: "0.4"
#   overlay_image: /assets/images/blocks_with_skips.png
  actions:
    - label: "Explore Projects"
      url: "#projects"
excerpt: "Exploring the intersection of Deep Learning and Visual Communication."
intro: 
  - excerpt: "Welcome to **VisualAI**, a portfolio of projects where complex AI concepts are explained visually. From neural network architectures to data-driven illustrations, this space brings together research, clarity, and design."
---

{% assign featured_projects = site.projects | sort: 'date' | reverse | slice: 0,3 %}

<div class="feature__wrapper">
  {% for project in featured_projects %}
    <div class="feature__item">
      <div class="feature__image">
        <a href="{{ project.url | relative_url }}">
          <img src="{{ project.image | relative_url }}" alt="{{ project.title }}">
        </a>
      </div>
      <h3 class="feature__title">{{ project.title }}</h3>
      <p>{{ project.excerpt | markdownify }}</p>
      <a href="{{ project.url | relative_url }}" class="btn btn--primary">View Project</a>
    </div>
  {% endfor %}
</div>