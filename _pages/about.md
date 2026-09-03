---
permalink: /
title: "About"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I’m **Tianze Xu (“徐天泽” in Chinese)**,  a second-year Ph.D. student at Shanghai Jiao Tong University, advised by [Prof. Pengfei Liu](https://plms.ai/). My research interests currently focuses on **fine-grained post-training** (Token-level reward assignment, On-Policy Distillation, etc.) and  LLM evaluation. I once interned at Alibaba (Taobao & Tmall Group) on agentic reinforcement learning.

## News

- **Jul 2026**: Two papers accepted by COLM 2026 — *Rubrics to Tokens* and *ResearcherBench*.
- **Apr 2026**: *Rubrics to Tokens: Bridging Response-level Rubrics and Token-level Rewards in Instruction Following Tasks* released on [arXiv](https://arxiv.org/abs/2604.02795).
- **Jul 2025**: *ResearcherBench: Evaluating Deep AI Research Systems on the Frontiers of Scientific Inquiry* (co-first author) released on [arXiv](https://arxiv.org/abs/2507.16280).
- **2025**: Started my Ph.D. at Shanghai Jiao Tong University, advised by Prof. Pengfei Liu.

## Publications

{% include base_path %}

<style>
.pub-tabs { display: flex; gap: 2px; border-bottom: 1px solid #e1e4e9; margin-bottom: 14px; }
.pub-tab { background: none; border: none; border-bottom: 2px solid transparent; padding: 6px 14px; cursor: pointer; font-size: 0.95em; color: #7a8288; font-family: inherit; }
.pub-tab.active { color: var(--global-theme-color, #3273dc); border-bottom-color: var(--global-theme-color, #3273dc); font-weight: 600; }
.pub-item { margin-bottom: 12px; }
.pub-title { font-size: 0.9em; font-weight: 600; color: var(--global-text-color, #494e52); text-decoration: none; }
.pub-title:hover { color: var(--global-theme-color, #3273dc); text-decoration: underline; }
.pub-meta { display: block; font-size: 0.85em; color: #7a8288; margin-top: 2px; }
</style>

<div class="pub-tabs">
  <button type="button" class="pub-tab active" onclick="showPubs('selected', this)">Selected</button>
  <button type="button" class="pub-tab" onclick="showPubs('all', this)">All Pubs</button>
</div>

{% assign selected_pubs = site.publications reversed | where: "selected", true %}

<div id="pubs-selected">
{% for post in selected_pubs %}
  <div class="pub-item">
    <a class="pub-title" href="{{ base_path }}{{ post.url }}">{{ post.title }}</a>
    <span class="pub-meta">{{ post.venue }}, {{ post.date | date: "%Y" }}</span>
  </div>
{% endfor %}
</div>

<div id="pubs-all" style="display: none;">
{% for post in site.publications reversed %}
  <div class="pub-item">
    <a class="pub-title" href="{{ base_path }}{{ post.url }}">{{ post.title }}</a>
    <span class="pub-meta">{{ post.venue }}, {{ post.date | date: "%Y" }}</span>
  </div>
{% endfor %}
</div>

<script>
function showPubs(which, btn) {
  document.getElementById('pubs-selected').style.display = (which === 'selected') ? 'block' : 'none';
  document.getElementById('pubs-all').style.display = (which === 'all') ? 'block' : 'none';
  document.querySelectorAll('.pub-tab').forEach(function (t) { t.classList.remove('active'); });
  btn.classList.add('active');
}
</script>

## Education

- **Ph.D. in Electronic Information (Artificial Intelligence)**, School of Computer Science and Engineering, Shanghai Jiao Tong University, 2025 – 2030 (expected)
  - Advisor: [Prof. Pengfei Liu](https://plms.ai/)
- **B.S.**, Beijing University of Posts and Telecommunications, 2021 – 2025
