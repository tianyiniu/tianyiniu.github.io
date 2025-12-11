---
layout: archive
title: "CV"
permalink: /cv/
author_profile: false
redirect_from:
  - /resume-json
---

{% include base_path %}

<style>
  /* Maximizes the width for the PDF viewer */
  .archive {
    width: 100% !important;
    padding-right: 0;
    margin-right: 0;
  }

  /* Responsive container for the PDF */
  .pdf-container {
    width: 100%;
    height: 85vh; /* Takes up 85% of the viewport height */
    border: 1px solid #ccc;
    border-radius: 4px;
    margin-bottom: 20px;
  }
</style>

<object data="{{ base_path }}/files/cv.pdf" type="application/pdf" class="pdf-container">
    <div style="padding: 20px; text-align: center;">
        <p>Your browser does not support embedded PDF viewing.</p>
        <a href="{{ base_path }}/files/cv.pdf" class="btn btn--primary">Click here to download the PDF</a>
    </div>
</object>
