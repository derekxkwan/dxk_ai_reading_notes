---
title: "Barwise Music Structure Analysis with the Correlation Block-Matching Segmentation Algorithm"
date: 2026-02-02T13:45:57-08:00
authors: ["Axel Marmoret", "Jérémy E. Cohen", "Frédéric Bimbot"]
year: 2023
tags: ["dynamic programming", "self-similarity matrix", "music", "audio", "boundary detection (music)", "log mel spectrogram", "vectorization", "spectrogram", "handcrafted features", "bar-aligned similarity", "bar-aligned", "music theory", "popular music", "formal analysis (music)"]
categories: ["non-neural network"]
paper_url: "https://transactions.ismir.net/articles/10.5334/tismir.167"
doi: "10.5334/tismir.167"
paper_src: "Transactions of the International Society for Music Information Retrieval"
bibkey: "marmoret_barwise_2023"
math: true
draft: false
---

## Summary
Creates a new representation called Barwise TF (time frequency) matrix with (number of bars) x (vectorized spectrogram) dimensions. Argues in favor of barwise vs beatwise alignment. Adds using autocorrelation SSM and RBF as ways to calculate self-similarity matrix. Finds boundaries in SSM using dynamic programming (optimal segmentation on more bars relies on optimal segmentations of less bars) based on summed similarity scores and penalties from deviating from expected segmentation lengths (multiples of 4 or 8 bars). Run on SALAMI and RWC-pop datasets.

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

