---
title: "Pattern Clustering in Monophonic Music by Learning a Non-Linear Embedding From Human Annotations"
date: 2026-02-02T13:45:57-08:00
authors: ["Timothy de Reuse", "Ichiro Fujinaga"]
year: 2019
tags: ["dbscan", "music", "human annotation", "monophonic (music)", "contrastive learning", "folk music", "contrastive", "mlp", "hand-crafted features", "symbolic music", "handcrafted features", "motif (music)", "music theory", "pattern discovery", "melodic (music)"]
categories: ["deep learning", "supervised", "clustering"]
paper_url: "https://zenodo.org/records/3527922"
doi: "10.5281/zenodo.3527922"
paper_src: "International Society for Music Information Retrieval Conference (ISMIR 2019)
Pages: 761-768
Publication Title: Proceedings of the 20th International Society for Music Information Retrieval Conference
Publisher: ISMIR"
bibkey: "dereuse_pattern_2019"
math: true
draft: false
---

## Summary
Seeks to discover repeated patterns in monphonic music (MTC-ANN) by extracting features from labeled patterns, and doing constrastive learning (MLP) where given a specific tune family, ground truth pairs come from same patterns, dissimilar pairs from different ground-truth patterns, and trivial patterns (dissimilar) are generated from SIARCT-C. Train on one tune family, test on another and use DBSCAN for clustering with k=3 for epsilon parameter. Findings show no much agreement with ground-truth patterns (don't cluster the same way) with best homogeneity being 0.56 with $\epsilon\_{25}$ and poor compleness scores (0.12)  for all points but better for significant points (0.69 for homogeneity, 0.67 for completeness). Notes that learned embeddings do better than PCA and that even SOTA pattern recognition has trouble aligning with ground truth (human annotation)

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

