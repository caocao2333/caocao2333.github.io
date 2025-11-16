---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* B.S. in Computer Science, University of Rochester, 2026

Experiences
======
* Fall 2025 - Present: Software Engineering Intern
  * AiFinSphere
  * Developed full-stack quantitative finance tools (React, Python), later refactoring the monolith into microservices (Docker, FastAPI) and optimizing the database schema to significantly reduce API latency while establishing a robust CI/CD pipeline.

* Summer 2025: Research Fellowship
  * Department of Computer Science, University of Rochester
  * Engineered an A/B testing framework by patching the llama.cpp build system to conduct a first-principles performance analysis of the Intel AMX accelerator, revealing its competitive advantage over high-end GPUs in the memory-bound decoding phase to inform dynamic scheduling strategies for heterogeneous LLM inference.

* Fall 2024 - Present: Teaching Assistant
  * Department of Computer Science, University of Rochester
  * Supported students in Computer Organization (CSC 252) by leading office hour sessions on topics like buffer overflows and cache simulation, providing detailed technical feedback, and co-authoring exam questions.

* Summer 2024: Summer Researcher
  * School of Integrated Circuit, Tsinghua University
  * Authored a technical review on Network-on-Chip (NoC) deadlock avoidance for chiplet-based systems by synthesizing technical papers, schematics, and teardown reports to compare the trade-offs between modular turn-restriction and high-performance virtual-channel designs.

* Summer 2023: Software Engineering Intern
  * Raysdata
  * Contributed to a team-built Java/Spring backend for a client-facing management system, analyzing the MySQL database and modifying modules to integrate new, client-requested features.

Publications
======
  {% comment %} Order: conferences, poster, manuscripts; newest first within each {% endcomment %}
  {% assign conf = site.publications | where: "category", "conferences" | sort: "date" | reverse %}
  {% assign posters = site.publications | where: "category", "poster" | sort: "date" | reverse %}
  {% assign manus = site.publications | where: "category", "manuscripts" | sort: "date" | reverse %}
  <ul>
    {% for post in conf %}
      {% include archive-single-cv.html %}
    {% endfor %}
    {% for post in posters %}
      {% include archive-single-cv.html %}
    {% endfor %}
    {% for post in manus %}
      {% include archive-single-cv.html %}
    {% endfor %}
  </ul>

<!-- Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul> -->

Skills
======
* Programming Languages:
  * Java
  * Python
  * C
  * ASM
  * Verilog
* Software & Tools:
  * Git
  * Docker
  * CLI
  * Linux (Fedora, Ubuntu)
  * Shell scripting
