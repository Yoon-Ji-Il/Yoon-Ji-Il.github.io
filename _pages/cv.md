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
* M.S. in Electrical Engineering and Computer Science, DGIST, 2026 – Present
* B.S. in Electronic Engineering, Inha University, 2022 – 2026

Research Interests
======
* Human Motion Modeling
* Robotics
* Vision-Language-Action (VLA) Models

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
