---
title: "Transformer Encoder Satisfiability: Complexity and Impact on Formal Reasoning"
collection: publications
permalink: /publication/iclr25_trans_sat
excerpt: 'TL;DR: We investigate the challenges and possibilities of formal reasoning for encoder-only transformers (EOT) by examining their satisfiability problem (SAT). We find SAT is undecidable for general EOT but identify decidable and NEXPTIME-hard scenarios for quantized EOT, highlighting the complexity of these cases.'
date: 2025-05-01
venue: 'ICLR'
paperurl: 'https://openreview.net/forum?id=VVO3ApdMUE'
citation: ''
---

We analyse the complexity of the satisfiability problem, or similarly feasibility problem, (trSAT) for transformer encoders (TE), which naturally occurs in formal verification or interpretation, collectively referred to as formal reasoning. We find that trSAT is undecidable when considering TE as they are commonly studied in the expressiveness community. Furthermore, we identify practical scenarios where trSAT is decidable and establish corresponding complexity bounds. Beyond trivial cases, we find that quantized TE, those restricted by fixed-width arithmetic, lead to the decidability of trSAT due to their limited attention capabilities. However, the problem remains difficult, as we establish scenarios where trSAT is NEXPTIME-hard and others where it is solvable in NEXPTIME for quantized TE. To complement our complexity results, we place our findings and their implications in the broader context of formal reasoning.


