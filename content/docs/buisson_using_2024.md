---
title: "Using Pairwise Link Prediction and Graph Attention Networks for Music Structure Analysis"
date: 2026-02-02T13:45:57-08:00
authors: ["Morgan Buisson", "Brian Mcfee", "Slim Essid"]
year: 2024
tags: ["popular music", "structure labeling (music)", "beat-aligned similarity", "chroma", "beat-aligned", "contrastive", "gnn", "music", "fine-tuning", "spectral clustering", "multi-representation", "min-cut", "music theory", "boundary detection (music)", "formal analysis (music)", "self-similarity matrix", "audio", "mfcc", "graph neural network", "spectrogram"]
categories: ["unsupervised", "probabilistic", "deep learning", "clustering"]
paper_url: "https://hal.science/hal-04665063"
doi: ""
paper_src: "International Society for Music Information Retrieval"
bibkey: "buisson_using_2024"
math: true
draft: false
---

## Summary
Calculates and labels sections through pairwise relationships between embeddings (beat-centric). Pairwise relationships are represented by a graph with edges same-segment, same-section, different-section. Features $\bm{X}$ are calculated from mel-spectrograms transformed into a new space from contrastive learning (from buisson\_repetition-based\_2023). A SSM $\bm{A}$ is calculated from these feature vectors using RBF which is used to enhance the embeddings (in update rule of the two GNN layers + MLP the contrastive features are fed into) in $\bm{X^{\prime}}$. An SSM $\bm{A^{\prime}}$ is calculated on new features $\bm{X^{\prime}}$ which is fed into dilated/1x1 conv layers to learn edge links which are refined using multi-scale attention to form $\bm{E}$ combined with learned positional embeddings $\bm{B}$ to form $\bm{E^{\prime}}$. Output from first GNN (first SSM) $\bm{X^{\prime}}$ is combined with output from conv/attention $\bm{E^{\prime}}$ into edge-conditioned GNN. The result is used to calculate boundaries (linear layer) and one of K labels (done through the last GNN layer approximating the mincut problem that spectral clustering does). Datasets are RWC-Pop and Harmonix

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

