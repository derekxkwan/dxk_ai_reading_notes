---
title: "Unsupervised Learning of Deep Features for Music Segmentation"
date: 2026-02-02T13:45:57-08:00
authors: ["Matthew C. McCallum"]
year: 2019
tags: ["convolutional", "beatles", "music boundary", "triplet loss", "self-similarity matrix", "music", "music theory", "audio", "beat-aligned similarity", "boundary detection (music)", "cnn", "representation learning", "segmentation", "beat-aligned", "contrastive", "cqt", "popular music", "formal analysis (music)"]
categories: ["unsupervised", "deep learning"]
paper_url: "https://ieeexplore.ieee.org/abstract/document/8683407"
doi: "10.1109/ICASSP.2019.8683407"
paper_src: "ICASSP 2019 - 2019 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)"
bibkey: "mccallum_unsupervised_2019"
math: true
draft: false
---

## Summary
Learns embeddings for music segmentation using contrastive learning on beat-synchronized CQT input by picking positive samples near in time (16 beats) and negative samples further away  (from 28 to 166 beats away). Calculates SSM through euclidean distance on embeddings and calculates boundaries using peak-to-mean ratio. Performed on BeatlesTUT dataset. Beats methods from Foote using Euclidean distance SSM (2000) and Serra et al. (2014) which does unsupervised as well using similarity. Biased sampling (using 2d Fourier coeffs of HPCPs) best.

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

