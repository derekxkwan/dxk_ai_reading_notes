---
title: "To Catch A Chorus, Verse, Intro, or Anything Else: Analyzing a Song with Structural Functions"
date: 2026-02-02T13:45:57-08:00
authors: ["Ju-Chiang Wang", "Yun-Ning Hung", "Jordan B. L. Smith"]
year: 2022
tags: ["convolutional", "pop", "music boundary", "music", "audio", "boundary detection (music)", "cnn", "neural network architecture development", "transformer", "non-bar/beat aligned similarity", "music theory", "popular music", "structure labeling (music)", "formal analysis (music)"]
categories: ["deep learning", "supervised"]
paper_url: "https://ieeexplore.ieee.org/abstract/document/9747252"
doi: "10.1109/ICASSP43922.2022.9747252"
paper_src: "ICASSP 2022 - 2022 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)"
bibkey: "wang_catch_2022"
math: true
draft: false
---

## Summary
Proposes two neural network architectures (both taking in the harmonic representation from won\_data-driven\_2020 for input)for the downstream task of music structure analysis (both boundary demarcation and individual labels like "chorus" for pop music using probability curves). HarmonicCNN (meant to model human perception) has 7 conv layers and 2 linear layers. SpecTNT has two levels of transformer encoders: spectral (extracts spectral feats via Frequency Class Tokens) and temporal (self-attention along time axis across FCTs). Starts with a two-dim ResNet. HarmonicCNN focuses on "instant" outputs (function label probs for center of time chunk) and SpecTNT on "multi-point" (function label probs for each time point in time chunk). SpecTNT does better on all metrics than HarmonicCNN. deep structure features + Spectral clustering best on F-measure of normalized entropy score. SpecTNT best on boundary detection (train on Salami-pop, RWC-pop, Isophonics; eval on Harmonix). Both models do not to well on Isophonics dataset compared to others but strong on Salami-Pop, RWC-Pop (cross dataset eval training on everything else).

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

