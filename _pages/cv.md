---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

[Download Full CV (PDF)](https://arbab.dev/files/my-resume.pdf)

Technical Skills
======
* **Machine Learning & AI**
  * Deep Learning (PyTorch, TensorFlow)
  * Computer Vision & Image Processing
  * Natural Language Processing
  * MLOps & Model Deployment
* **Software Engineering**
  * Python, Java, C++
  * Distributed Systems
  * Cloud Computing (AWS, GCP)
  * System Design & Architecture
* **Tools & Technologies**
  * Git, Docker, Kubernetes
  * CI/CD Pipelines
  * Database Systems
  * RESTful APIs

Experience
======
* **Advanced Software Engineering Intern** (2023.05 - Present)
  * Kingland Systems
  * Developed enterprise-scale AI solutions
  * Implemented production ML pipelines
  * Tech stack: Python, AWS, Docker

* **Research Assistant** (2023.01 - Present)
  * AI Institute for Resilient Agriculture (AIIRA), Iowa State University
  * Led development of vision-language models for specialized tasks
  * Designed scalable 3D reconstruction systems
  * Tech stack: PyTorch, Computer Vision, MLOps

Education
======
* **Ph.D. in Computer Science**, Iowa State University (2022 - Present)
  * Focus: Machine Learning, Computer Vision, AI Systems
  * Advisor: Prof. Soumik Sarkar

Selected Publications
======
* **2024**: "Leveraging Vision Language Models for Specialized Agricultural Tasks" (WACV)
* **2024**: "Assisted Few-Shot Learning for Vision-Language Models" (NeurIPS Workshop)
* **2023**: "Mutation-based Fault Localization of Deep Neural Networks" (ASE) - Distinguished Paper Award

Projects & Open Source
======
{% for post in site.portfolio %}
  {% include archive-single-cv.html %}
{% endfor %}

Awards & Recognition
======
* Distinguished Paper Award, ASE 2023
* [Add your other awards here]
