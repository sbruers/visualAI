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

{% assign featured_projects = site.projects | sort: 'date' | reverse %}
<div class="grid__wrapper">
  {% for project in featured_projects %}
    <div class="grid__item">
      <a href="{{ project.url | relative_url }}">
        <img src="{{ project.image | relative_url }}" alt="{{ project.title }}">
        <h3>{{ project.title }}</h3>
      </a>
      <p>{{ project.excerpt }}</p>
    </div>
  {% endfor %}
</div>