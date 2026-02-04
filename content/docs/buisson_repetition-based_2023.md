---
title: "A Repetition-based Triplet Mining Approach for Music Segmentation"
date: 2026-02-02T13:45:57-08:00
authors: ["Morgan Buisson", "Brian Mcfee", "Slim Essid", "Helene-Camille Crayencour"]
year: 2023
tags: ["music theory", "audio", "formal analysis (music)", "beat-aligned", "beat-aligned similarity", "mfcc", "multi-representation", "popular music", "spectrogram", "chroma", "representation learning", "music", "contrastive", "jazz", "spectral clustering", "self-similarity matrix", "boundary detection (music)"]
categories: ["unsupervised", "clustering", "probabilistic"]
paper_url: "https://hal.science/hal-04202766"
doi: ""
paper_src: "Proceedings of ISMIR 2023"
bibkey: "buisson_repetition-based_2023"
math: true
draft: false
---

## Summary
frames (instead of just 1 vector). The resulting SSM is blurred with a gaussian kernel. Positive samples come from the SSM directly, negative samples come from 1 - SSM but using an exponential to weight nearby frames more heavily. Actual segmentation is spectral clustering. Uses SALAMI and Jazz Structure Datasets. Performs better than temporal sampling and laplacian structural decomposition.

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

