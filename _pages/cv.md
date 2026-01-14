---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* M.S. in Computer Science, KAIST (Mar. 2026 - present)
* B.S. in Mathematical Science & Computer Science (Double Major), KAIST (Mar. 2021 - Feb. 2026)
* Spring 2023 eschange at TU Berlin

Work experience
======
* Fall 2024 - Fall 2025: Undergraduate Lab Intern
  * KAIST VLLab
  * Duties includes: Research support and experiments in geometric deep learning projects
  * Supervisor: Prof. Seunghoon Hong, Mentor: Jinwoo Kim

Skills
======
* Programming & Libraries
  * Python (Pytorch, NumPy, HuggingFace) 
* Mathematical Tools
  * (Linear) Algebra, Differential Geometry, Topology

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
