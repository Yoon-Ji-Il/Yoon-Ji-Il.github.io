---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<style>
.cv-item { margin: 0 0 1.1em; }
.cv-head { display: flex; justify-content: space-between; gap: 1em; align-items: baseline; }
.cv-title { font-weight: 700; color: #1f2937; }
.cv-date { flex-shrink: 0; white-space: nowrap; font-size: 0.85em; color: #6b7280; }
.cv-sub { font-size: 0.9em; font-style: italic; color: #4b5563; margin-top: 0.15em; }
.cv-desc { font-size: 0.88em; color: #374151; margin-top: 0.35em; line-height: 1.55; }
.cv-venue { font-size: 0.88em; font-weight: 700; color: #1d4ed8; margin-top: 0.2em; }
.cv-skill { font-size: 0.9em; margin: 0 0 0.4em; }
.cv-skill b { display: inline-block; min-width: 9em; color: #1f2937; }
html[data-theme="dark"] .cv-title, html[data-theme="dark"] .cv-skill b { color: #f3f4f6; }
html[data-theme="dark"] .cv-sub, html[data-theme="dark"] .cv-desc, html[data-theme="dark"] .cv-date { color: #d1d5db; }
html[data-theme="dark"] .cv-venue { color: #93c5fd; }
@media (max-width: 600px) { .cv-head { flex-direction: column; gap: 0.1em; } }
</style>

## Education

<div class="cv-item">
<div class="cv-head"><span class="cv-title">M.S. in Electrical Engineering and Computer Science</span><span class="cv-date">2026.09 – Present</span></div>
<div class="cv-sub">DGIST (Daegu Gyeongbuk Institute of Science and Technology), Daegu, Korea</div>
</div>

<div class="cv-item">
<div class="cv-head"><span class="cv-title">B.S. in Electronic Engineering</span><span class="cv-date">2022.02 – 2026.02</span></div>
<div class="cv-sub">Inha University, Incheon, Korea</div>
</div>

## Research Interests

<div class="cv-desc">Human Motion Modeling · Robotics · Vision-Language-Action (VLA) Models</div>

## Publications

{% assign pubs = site.publications | sort: "date" | reverse %}
{% for post in pubs %}
<div class="cv-item">
<div class="cv-title">{{ post.title }}</div>
<div class="cv-desc">{{ post.authors }}</div>
<div class="cv-venue">{{ post.venue_short | default: post.venue }} ({{ post.date | date: "%Y" }})</div>
</div>
{% endfor %}

<div class="cv-desc">* Equal contribution &nbsp; † Corresponding author</div>

## Research Experience

<div class="cv-item">
<div class="cv-head"><span class="cv-title">Forklift Safety System Project (with CJ)</span><span class="cv-date">2025.08 – Present</span></div>
<div class="cv-sub">SPARO Lab, Inha University</div>
<div class="cv-desc">Fused data from a 360° camera (Ricoh Theta) and a LiDAR (Mid-360) to detect people around forklifts and prevent safety accidents in a CJ factory.</div>
</div>

<div class="cv-item">
<div class="cv-head"><span class="cv-title">Optimization and Verilog HDL Implementation of Sub-Modules for YOLOv5</span><span class="cv-date">2025.01 – 2025.07</span></div>
<div class="cv-sub">Undergraduate Thesis, Inha University</div>
<div class="cv-desc">Implemented YOLOv5 sub-modules in Verilog HDL and designed a processing element (PE) architecture. Showed that the hardware implementation ran faster than GPU-based execution.</div>
</div>

## Honors & Awards

<div class="cv-item">
<div class="cv-head"><span class="cv-title">Excellence Award, Advantech Inno-Works Project 2024</span><span class="cv-date">2024</span></div>
<div class="cv-sub">Advantech · Inha University</div>
<div class="cv-desc">Team "냉장고를 부탁해" (Please Take Care of My Refrigerator). Built a system to reduce a refrigerator's power consumption and carbon footprint by measuring its internal volume with a 3D depth camera and recognizing items through MMOCR-based object detection, text recognition, and tracking.</div>
</div>

<div class="cv-item">
<div class="cv-head"><span class="cv-title">Certificate of Completion, Samsung Dream Class</span><span class="cv-date">2023.02 – 2024.02</span></div>
<div class="cv-sub">Samsung</div>
<div class="cv-desc">Completed a one-year educational volunteer program run by Samsung.</div>
</div>

## Skills

<div class="cv-skill"><b>Programming</b>Python, C/C++, Verilog</div>
<div class="cv-skill"><b>Robotics &amp; Tools</b>ROS 1/2, Docker</div>
<div class="cv-skill"><b>Hardware</b>FPGA (Zybo, UltraScale)</div>
