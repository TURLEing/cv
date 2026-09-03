---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

[Download CV as PDF]({{ base_path }}/files/cv.pdf){: .btn .btn--primary}

## Education

* **Ph.D. in Electronic Information (Artificial Intelligence)**, School of Computer Science and Engineering, Shanghai Jiao Tong University, 2025 – 2030 (expected)
  * Advisor: Prof. Pengfei Liu
* **B.S. in E-Commerce and Law**, International School, Beijing University of Posts and Telecommunications, 2021 – 2025
  * National Scholarship (2021); University Second-Class Scholarship and Merit Student (2022)

## Work Experience

* **Oct 2025 – Sep 2026: Large Language Model Algorithm Intern**, Alibaba Group, Taobao & Tmall Group, Business Technology Team
  * Conducted Agent-RL research on fine-grained reward modeling and credit assignment for complex instruction following, leading to the first-author COLM 2026 paper *Rubrics to Tokens*.
  * Built an end-to-end distributed training pipeline on ROLL (data construction, token-level discriminator training/inference, advantage estimation, policy updates, automated evaluation) supporting multiple Qwen and Llama configurations.
  * Drove RTT's rollout into the e-commerce data-analysis Agent loop with a hybrid reward (rule signals + expert rubrics + LLM-as-Judge) localized onto key content tokens, reasoning steps, and tool behaviors.
* **May – Sep 2023: Algorithm Intern**, Lingxin Intelligence
  * Contributed to **CharacterGLM**, an empathetic persona-consistent model released jointly with Tsinghua's CoAI Lab; built a large-scale distillation annotation pipeline over frontier LLMs to synthesize, clean, and label personalized dialogue data.

## Awards

* First Prize, Beijing Division, 13th and 14th Lanqiao Cup (Software, Group A), 2022 / 2023
* First Prize, Beijing Division, China International College Students' Innovation Competition ("Painting Music with Colors"), 2024

## Publications

<ul>{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>
