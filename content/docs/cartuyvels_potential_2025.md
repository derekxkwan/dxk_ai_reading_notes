---
title: "The Potential of Unsupervised Induction of Harmonic Syntax for Jazz"
date: 2026-02-02T13:45:57-08:00
authors: ["Ruben Cartuyvels", "John Koslovsky", "Marie-Francine Moens"]
year: 2025
tags: ["harmonic analysis (music)", "hierarchical analysis", "parse trees", "music", "jazz", "hierarchy", "romantic period (music)", "pcfg", "classical period (music)", "mlp", "harmony (music)", "symbolic music", "context-free grammar", "music theory", "popular music", "classical music"]
categories: ["classification", "unsupervised", "probabilistic", "deep learning"]
paper_url: ""
doi: "10.5334/tismir.217"
paper_src: "Transactions of the International Society for Music Information Retrieval"
bibkey: "cartuyvels_potential_2025"
math: true
draft: false
---

## Summary
Models a probabilistic context-free grammar using three neural networks ($S \rightarrow A$, $A \rightarrow B\_1, B\_2$, $P \rightarrow c$ where $c$ is chord). Used the chord embeddings of foscarin\_predicting\_2023 without duration and metrical strength. Optionally train to optimize rules (dominant to tonic etc) or chord relations (root relations) using negative log-likelihood. Uses JHT dataset and ChoCo. Trained unsupervised, does not do as well as foscarin\_predicting\_2023 but not terribly.

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

