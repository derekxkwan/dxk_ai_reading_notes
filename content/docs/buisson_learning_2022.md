---
title: "Learning Multi-Level Representations for Hierarchical Music Structure Analysis"
date: 2026-02-02T13:45:57-08:00
authors: ["Morgan Buisson", "Brian Mcfee", "Slim Essid", "Helene-Camille Crayencour"]
year: 2022
tags: ["convolutional", "jazz", "popular music", "beat-aligned similarity", "music boundary", "cnn", "log-mel", "representation learning", "segmentation", "beat-aligned", "contrastive", "music", "spectral clustering", "multi-level", "music theory", "boundary detection (music)", "formal analysis (music)", "hierarchical analysis", "audio"]
categories: ["unsupervised", "deep learning", "clustering"]
paper_url: "https://hal.science/hal-03780032"
doi: ""
paper_src: "Proceedings of ISMIR 2022"
bibkey: "buisson_learning_2022"
math: true
draft: false
---

## Summary
Uses log-mel spectrograms and similarly to mccallum\_unsupervised\_2019, does unsupervised triplet-loss to learn representations for boundary detection (spectral clustering). Unlike McCallum, does sampling of positives at various levels of granularity. With each finer level, the positive window shrinks and the positive samples from the previous layer is used as the negative sample of the finer layer. Learns through Conditional Similarity Networks (masks out part of embedding space for each level of coarseness). Performed on BeatlesTUT, RWC-Pop, RWC-Jazz, JAAH (Jazz Audio-Aligned Harmony from "The Smithsonian Collection of Classic Jazz" and "Jazz: The Smithsonian Anthology").  Compared to mccallum\_unsupervised\_2019 and Nieto/Bello 2019 and mcfee\_analyzing\_2014. Performs worse on lower (aside from Nieto/Bello) except for "best results across all levels" but performs  better on upper. Performs competitively (but overall slightly lower) on multi-level compared to Tralie/McFee 2019, McFee/Nieto/arbood/Bello 2017 and  Salomon/Nieto/Bryan 2021 (except ofr "best")

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

