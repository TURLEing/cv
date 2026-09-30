---
title: "MOPD-Router: Rethinking Teacher Routing in Multi-Teacher On-Policy Distillation"
authors: ["Tianze Xu", "Yanzhao Zheng", "Zhentao Zhang", "Yuanqiang Yu", "Chao Ma", "Jihuai Zhu", "Lelun Wu", "Lyumanshan Ye", "Pengfei Liu", "Baohua Dong", "Hangcheng Zhu", "Ruohui Huang", "Gang Yu"]
collection: publications
category: conferences
selected: true
permalink: /publication/mopd-router/
excerpt: "A label-free, token-level teacher-routing framework for multi-teacher on-policy distillation."
date: 2026-09-25
venue: "arXiv preprint"
paperurl: "https://arxiv.org/abs/2609.30837"
citation: "Xu, T., Zheng, Y., Zhang, Z., Yu, Y., Ma, C., Zhu, J., Wu, L., Ye, L., Liu, P., Dong, B., Zhu, H., Huang, R., &amp; Yu, G. (2026). &quot;MOPD-Router: Rethinking Teacher Routing in Multi-Teacher On-Policy Distillation.&quot; arXiv:2609.30837."
---

MOPD-Router routes supervision from a pool of specialized teachers at each token, without prompt-level domain labels or a separately trained routing model. Its ExpertAlign metric weights each teacher's correction according to how well it reflects that teacher's post-training specialization. Across four distillation settings, ExpertAlign achieved the strongest overall performance; on unlabeled training data, it improved the overall score by 5.88 points over mean aggregation.

[arXiv](https://arxiv.org/abs/2609.30837) · [Code](https://github.com/TURLEing/MOPD-Router)
