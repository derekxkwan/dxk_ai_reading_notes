---
title: "AutoSchA: Automatic Hierarchical Music Representations via Multi-Relational Node Isolation"
date: 2026-02-09T21:01:30-08:00
authors: ["Stephen Ni-Hahn", "Rico Zhu", "Jerry Yin", "Yue Jiang", "Cynthia Rudin", "Simon Mak"]
year: 2025
tags: ["schenker", "schenkerian", "graph neural network", "music theory", "music analysis", "music", "hierarchical music analysis", "symbolic music"]
categories: ["deep learning", "supervised"]
paper_url: ""
doi: "10.48550/arXiv.2512.18232"
paper_src: "arXiv"
bibkey: "nihahn2025"
math: true
draft: false
---

## Summary
Describes a graph neural network with novel graph pooling layer (like CNN pooling layer) which scores each node (note) with a vector $\hat{\bm{y}}$ to drop with each layer, giving a Schenkerian depth. Uses a global feature aggregation technique implemented by a transformer encoder on input features to give enhanced node embeddings. Also uses a subspace merging approach by using an undirected graph representation $\hat{\bm{A}_i}$ that is convolved with initial embeddings. Trained using SchA from nihahn2024 and outperforms GCNs, Graph Attention Networks, and R-GCNs.
## Key Contributions
Novel graph pooling mechanism to determine Schenkerian depths of notes. Incorporation of global graph info through global feature aggregation and subspace merging.

## Limitations and Future Work
Yields "awkward components" to humans at times.

## Key Equations
$\hat{\bm{y}} = \sigma (\sum\limits_{i=1}^{m} (\alpha \widetilde{\bm{M_i}} \bm{Z} \bm{W_{i,\rightarrow}} + \bar{\alpha} \widetilde{\bm{M_i^T}}\bm{Z} \bm{W_{i,\leftarrow}}))$

($\bm{Z}$ node embedding matrix, $\bm{W_i}$ forward and backward learned weights, $\widetilde{\bm{M}} = \widetilde{\bm{D}^{-\frac{1}{2}}} \widetilde{\bm{A}} \widetilde{\bm{D}^{-\frac{1}{2}}}$, $\widetilde{\bm{D}}$ degree matrix, $\widetilde{\bm{A}} = \bm{A} + \bm{I_n}$ self-loop adj matrix)


## Other Notes
