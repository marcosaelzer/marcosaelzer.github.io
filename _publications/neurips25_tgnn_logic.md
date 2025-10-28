---
title: "The Logical Expressiveness of Temporal GNNs via Two-Dimensional Product Logics"
collection: publications
permalink: /publication/neurips25_tgnn_logic
excerpt: 'TL;DR: We establish (some) characterisations of the expressive capabilities of different TGNN models based on product logics.'
date: 2025-10-01
venue: 'NeurIPS'
paperurl: 'https://openreview.net/forum?id=v13yQBxhut'
---

In recent years, the expressive power of various neural architectures---including graph neural networks (GNNs), transformers, and recurrent neural networks---has been characterised using tools from logic and formal language theory. As the capabilities of basic architectures are becoming well understood, increasing attention is turning to models that combine multiple architectural paradigms. Among them particularly important, and challenging to analyse, are temporal extensions of GNNs, which integrate both spatial (graph-structure) and temporal (evolution over time) dimensions. In this paper, we initiate the study of logical characterisation of temporal GNNs by connecting them to two-dimensional product logics. We show that the expressive power of temporal GNNs depends on how graph and temporal components are combined. In particular, temporal GNNs that apply static GNNs recursively over time can capture all properties definable in the product logic of (past) propositional temporal logic PTL and the modal logic K. In contrast, architectures such as graph-and-time TGNNs and global TGNNs can only express restricted fragments of this  logic, where the interaction between temporal and spatial operators is syntactically constrained. These provide us with the first results on the logical expressiveness of temporal GNNs.

