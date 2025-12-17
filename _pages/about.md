---
permalink: /
title: "Tianyi Niu"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
.page__content { font-size: 0.85em; } 
</style>


Hello! I am pursuing a Master of Science in Computer Science at [The University of North Carolina at Chapel Hill](https://www.unc.edu). I am currently a Research Assistant at [MURGe-Lab](https://murgelab.cs.unc.edu), advised by [Prof. Mohit Bansal](https://www.cs.unc.edu/~mbansal/) and Prof. [Elias Stengel-Eskin](https://esteng.github.io/). **I am applying to PhD programs starting Fall 2026.** 

My current research focuses on two key directions: 
1. **Abstractions and Cognition of MLLMs.** How do abstractions formed by (M)LLMs differ from humans,
and can insights from human cognition inform model development, and vice versa?
1. **Interaction and communication in multi-agent systems.** How is knowledge transferred in multi-agent
systems, and can principles of human communication also inform and optimize multi-agent interaction
paradigms?

I previously graduated from UNC Chapel Hill highest distinction, obtaining a BS in Computer Science with highest honors and a BA in Linguistics. My undergraduate thesis (advised by [Prof. Shashank Srivastava](https://www.ssriva.com)) explored whether LLMs benefit from curriculum training on synthetic pre-training data.

Feel free to reach me at: tianyin4 [at] cs [dot] unc [dot] edu

## 📢 News

<div class="about-content">
  <div class="news-box"> 
    
    <div class="news-item">
      <div class="news-date">Aug 21, 2025</div>
      <div class="news-content">
        New preprint: <i>RotBench: Evaluating Multimodal Large Language Models on Identifying Image Rotation</i>.
      </div>
    </div>

    <div class="news-item">
      <div class="news-date">Aug 20, 2025</div>
      <div class="news-content">
        1 paper accepted into <strong>EMNLP 2025</strong>: <i>Chameleon LLMs: User Personas Influence ChatBot Personality Shifts</i>.
      </div>
    </div>

    <div class="news-item">
      <div class="news-date">June 01, 2025</div>
      <div class="news-content">
        Joined MURGe-Lab as a Research Assistant advised by Prof. Mohit Bansal.
      </div>
    </div>

  </div> </div>


## 📝 Publications

<div class="about-content">
  {% assign sorted_pubs = site.publications | sort: 'date' | reverse %}
  {% for post in sorted_pubs %}
    
    {% assign venue_down = post.venue_nickname | downcase %}
    {% if venue_down contains 'neurips' %}
      {% assign badge_class = 'badge-neurips' %}
      {% assign badge_text = 'NeurIPS' %}
    {% elsif venue_down contains 'emnlp' %}
      {% assign badge_class = 'badge-emnlp' %}
      {% assign badge_text = 'EMNLP' %}
    {% elsif venue_down contains 'colm' %}
      {% assign badge_class = 'badge-colm' %}
      {% assign badge_text = 'COLM' %}
    {% elsif venue_down contains 'icimth' %}
      {% assign badge_class = 'badge-icimth' %}
      {% assign badge_text = 'ICIMTH' %}
    {% elsif venue_down contains 'arxiv' %}
      {% assign badge_class = 'badge-arxiv' %}
      {% assign badge_text = 'Preprint' %}
    {% elsif venue_down contains 'acl' %}
      {% assign badge_class = 'badge-acl' %}
      {% assign badge_text = 'ACL' %}
    {% elsif venue_down contains 'sigmorphon' %}
      {% assign badge_class = 'badge-sigmorphon' %}
      {% assign badge_text = 'sigmorphon' %}
    {% elsif venue_down contains 'thesis' %}
      {% assign badge_class = 'badge-thesis' %}
      {% assign badge_text = 'Thesis' %}
    {% else %}
      {% assign badge_class = 'badge-default' %}
      {% assign badge_text = 'Paper' %} 
    {% endif %}

    <div class="pub-item">
      <div class="pub-badge {{ badge_class }}">
        {{ badge_text }}
      </div>

      <div class="pub-content">
        <a href="{{ post.paperurl | default: post.url }}" class="pub-title">
        {{ post.title }}
        </a>
        
        <div class="pub-authors">
          {{ post.authors | default: "Authors List Placeholder" }}
        </div>
        
        <div class="pub-venue">
          {{ post.venue }}
        </div>
      </div>
      <div class="pub-year-bg">{{ post.date | date: "%Y" }}</div>
    </div>
  {% endfor %}
</div>