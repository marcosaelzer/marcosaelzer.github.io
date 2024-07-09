---
title: "The Computational Complexity of Formal Reasoning for Encoder-Only Transformers"
collection: publications
permalink: /publication/arxiv24_trans_sat
excerpt: 'TL;DR: We investigate the challenges and possibilities of formal reasoning for encoder-only transformers (EOT) by examining their satisfiability problem (SAT). We find SAT is undecidable for general EOT but identify decidable and NEXPTIME-hard scenarios for quantized EOT, highlighting the complexity of these cases.'
date: 2024-05-28
venue: 'arXiv'
paperurl: 'https://arxiv.org/abs/2405.18548'
citation: ''
---

We investigate challenges and possibilities of formal reasoning for encoder-only transformers (EOT), meaning sound and complete methods for verifying or interpreting behaviour. In detail, we condense related formal reasoning tasks in the form of a naturally occurring satisfiability problem (SAT). We find that SAT is undecidable if we consider EOT, commonly considered in the expressiveness community. Furthermore, we identify practical scenarios where SAT is decidable and establish corresponding complexity bounds. Besides trivial cases, we find that quantized EOT, namely those restricted by some fixed-width arithmetic, lead to the decidability of SAT due to their limited attention capabilities. However, the problem remains difficult, as we establish those scenarios where SAT is NEXPTIME-hard and those where we can show that it is solvable in NEXPTIME for quantized EOT. To complement our theoretical results, we put our findings and their implications in the overall perspective of formal reasoning.


