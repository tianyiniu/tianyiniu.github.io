---
title: "Socratic Students: Teaching Language Models to Learn by Asking Questions"
collection: publications
category: manuscripts
permalink: /publication/2025-12-15-socraticstudents
excerpt: ''
date: 2025-12-15
venue: 'Arxiv preprint'
venue_nickname: 'arxiv'
authors: 'Rajeev Bhatt Ambati, <u>Tianyi Niu*</u>, Aashu Singh, Shlok Mishra, Shashank Srivastava, Snigdha Chaturvedi'
paperurl: "https://arxiv.org/abs/2512.13102"
# slidesurl: 'http://academicpages.github.io/files/slides1.pdf'
# paperurl: 'http://academicpages.github.io/files/paper1.pdf'
# bibtexurl: 'http://academicpages.github.io/files/bibtex1.bib'
# citation: 'Your Name, You. (2009). &quot;Paper Title Number 1.&quot; <i>Journal 1</i>. 1(1).'
---

**Authors**

Rajeev Bhatt Ambati, <u>Tianyi Niu*</u>, Aashu Singh, Shlok Mishra, Shashank Srivastava, Snigdha Chaturvedi

**Abstract**

Large Language Models (LLMs) excel at static interactions, where they answer user queries by retrieving knowledge encoded in their parameters. However, in many real-world settings, such as educational tutoring or medical assistance, relevant information is not directly available and must be actively acquired through dynamic interactions. An interactive agent would recognize its own uncertainty, ask targeted questions, and retain new knowledge efficiently. Prior work has primarily explored effective ways for a teacher to instruct the student, where the teacher identifies student gaps and provides guidance. In this work, we shift the focus to the student and investigate effective strategies to actively query the teacher in seeking useful information. Across math and coding benchmarks, where baseline student models begin with near-zero performance, we show that student-led approaches consistently yield absolute Pass@k improvements of at least 0.5 over static baselines. To improve question quality, we train students using Direct Preference Optimization (DPO) with guidance from either self or stronger students. We find that this guided training enables smaller models to learn how to ask better questions, further enhancing learning efficiency.

**Paper**: [https://arxiv.org/abs/2512.13102](https://arxiv.org/abs/2512.13102)
