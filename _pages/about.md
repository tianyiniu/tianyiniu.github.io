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

<style>
  .news-box {
    /* 1. Sizing & Scrolling */
    height: 200px; /* Fixed height */
    overflow-y: scroll; /* Forces scrollbar to appear */
    
    /* 2. Border & Design */
    border: 1px solid #e1e4e8; /* Light gray border */
    border-radius: 6px; /* Rounded corners */
    padding: 15px; /* Spacing inside the border */
    background-color: #f6f8fa; /* Very faint gray background */
    box-shadow: inset 0 1px 2px rgba(0,0,0,0.03); /* Subtle inner shadow */
    font-size: 0.9em; 
  }

  .news-item {
    display: flex;
    flex-direction: row;
    margin-bottom: 12px;
    border-bottom: 1px solid #eaecef; /* Optional separator line between items */
    padding-bottom: 12px;
  }
  
  /* Removes the line from the last item */
  .news-item:last-child {
    border-bottom: none;
    margin-bottom: 0;
    padding-bottom: 0;
  }

  .news-date {
    flex: 0 0 85px; /* Width of the date column */
    font-weight: 600;
    color: #444;
    padding-right: 10px;
    font-size: 0.85em;
  }
  
  .news-content {
    flex: 1;
    color: #24292e;
  }
  
  /* Link styling inside the box */
  .news-content a {
    color: #0366d6;
    text-decoration: none;
  }
  .news-content a:hover {
    text-decoration: underline;
  }
</style>

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

</div>


## 📝 Publications

<style>
  /* 1. Container for the list */
  .pub-list {
    display: flex;
    flex-direction: column;
    gap: 20px; /* Space between papers */
  }

  /* 2. Each Paper Row */
  .pub-item {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    position: relative;
  }

  /* 3. The Badge (Left Side) */
 .pub-badge {
    width: 80px;
    padding: 3px 0; /* Slightly less padding because of the border */
    text-align: center;
    font-weight: 600;
    font-size: 0.6em;
    border-radius: 4px;
    margin-right: 20px;
    flex-shrink: 0;
    text-transform: uppercase;
    letter-spacing: 1px;
    
    /* The Subtle Changes: */
    box-shadow: none;
    background-color: transparent; /* See-through background */
    border: 1px solid #e5e7eb; /* Default light border */
    }

  /* Badge Colors - Add more as needed */
    /* Big AI: ICLR, ICML, NeurIPS, COLM */
    .badge-neurips,
    .badge-icml,
    .badge-iclr,
    .badge-colm { 
    border-color: #9333ea; 
    color: #9333ea; 
    }
    /* NLP and Comp Ling Oriented: ACL, NAACL, EACL, SIGMORPHON */
    .badge-acl,
    .badge-naacl,
    .badge-eacl,
    .badge-emnlp,
    .badge-sigmorphon { 
    border-color: #0d9488; 
    color: #0d9488; 
    }
    /* Healthcare: ICIMTH */
    .badge-icimth { 
    border-color: #ea580c; 
    color: #ea580c; 
    }
    /* Other (thesis, preprints) */
    .badge-arxiv,
    .badge-thesis { 
    border-color: #2563eb; 
    color: #2563eb; 
    }
    /* Default */
    .badge-default { 
    border-color: #64748b; 
    color: #64748b; 
    }

  /* 4. The Content (Right Side) */
  .pub-content {
    flex-grow: 1;
  }

  .pub-title {
    font-weight: 600;
    color: #c026d3; /* Matches your theme color */
    text-decoration: none;
    font-size: 1.0em;
    display: block;
    margin-bottom: 4px;
    margin-right: 2px;
  }
  
  .pub-title:hover {
    text-decoration: underline;
  }

  .pub-authors {
    color: #333;
    font-size: 0.8em;
    margin-bottom: 2px;
  }

  .pub-venue {
    color: #666;
    font-size: 0.7em;
  }

</style>

<div class="pub-list">
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