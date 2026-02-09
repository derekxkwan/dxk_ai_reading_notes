---
title: "Self-Similarity-Based and Novelty-based loss for music structure analysis"
date: 2026-02-02T13:45:57-08:00
authors: ["Geoffroy Peeters"]
year: 2023
tags: ["self-similarity matrix", "music", "audio", "boundary detection (music)", "log mel spectrogram", "cnn", "transformer", "representation learning", "non-bar/beat aligned similarity", "music theory", "popular music", "formal analysis (music)", "log-mel spectrogram"]
categories: ["deep learning", "supervised"]
paper_url: "https://telecom-paris.hal.science/hal-04155178"
doi: ""
paper_src: ""
bibkey: "peeters_self-similarity-based_2023"
math: true
draft: false
---

## Summary
Learns (non-beat aligned) vectorized features for a SSM from log-mel spectrograms into convolutional layers and uses self-attention to incorporate information from other embeddings. Calculates the SSM through scaled-cosine similarity and uses BCE weighted loss (since more 0s than 1s in ground truth). Adds another convolutional layer to learn kernel on top of SSM to calculate novelty scores which are init random or with checkerboard. Uses peak-to-mean ratio algo to get segments from novelty scores. Experiments with RCW-POP-AIST, SA-POP, SA-IA, SA-Two (SALAMI). Outperforms baselines on SA-Pop, SA-IA, but buisson\_learning\_2022 does better on SA-Two, grill\_music\_2015 does better on RWC-PopAIST with hit rate on 3s, mccallum\_unsupervised\_2019 better on hit-rate 3s for SA-Pop.

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

