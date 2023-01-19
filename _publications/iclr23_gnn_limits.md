---
title: "Fundamental Limits in Formal Verification of Message-Passing Neural Networks"
collection: publications
permalink: /publication/arxiv2_gnnlimits
excerpt: 'TL;DR: We proof that formal verification of different safety properties of graph-classifying MPNN is impossible in general and that verification problems for
node-classifying GNN are solvable if the considered graphs have bounded degree.' 
date: 2022-10-04
venue: 'arXiv'
paperurl: 'https://arxiv.org/abs/2206.05070'
citation: ''
---
Output reachability and adversarial robustness are among the most relevant safety properties of neural networks. We show that in the context of Message Passing Neural Networks (MPNN), a common Graph Neural Network (GNN) model, formal verification is impossible. In particular, we show that output reachability of graph-classifier MPNN, working over graphs 
of unbounded size, non-trivial degree and sufficiently expressive node labels, cannot be verified formally: there is no algorithm that answers correctly (with yes or no), given an MPNN, whether there exists some valid input to the MPNN such that the corresponding output satisfies a given specification. However, we also show that output reachability and 
adversarial robustness of node-classifier MPNN can be verified formally when a limit on the degree of input graphs is given a priori. We discuss the implications of these results, for the purpose of obtaining a complete picture of the principle possibility to formally verify GNN, depending on the expressiveness of the involved GNN models and input-output 
specifications. 

[arXiv version](https://arxiv.org/pdf/2206.05070.pdf)

