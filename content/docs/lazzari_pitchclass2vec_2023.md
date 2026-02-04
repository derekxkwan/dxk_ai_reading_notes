---
title: "Pitchclass2vec: Symbolic Music Structure Segmentation with Chord Embeddings"
date: 2026-02-02T13:45:57-08:00
authors: ["Nicolas Lazzari", "Andrea Poltronieri", "Valentina Presutti"]
year: 2023
tags: ["harmonic analysis (music)", "music theory", "formal analysis (music)", "structure labeling (music)", "pitch classes", "popular music", "representation learning", "segmentation", "music", "symbolic music", "language-inspired (music)", "word2vec", "rnn", "fasttext", "boundary detection (music)"]
categories: ["deep learning"]
paper_url: "https://ui.adsabs.harvard.edu/abs/2023arXiv230315306L"
doi: "10.48550/arXiv.2303.15306"
paper_src: "Proceedings of the 1st Workshop on Artificial Intelligence and Creativity"
bibkey: "lazzari_pitchclass2vec_2023"
math: true
draft: false
---

## Summary
Learns a chord representation based on ideas of fasttext (same was word2vec training but splits words into n-grams first and then words are sums of their n-grams). Instead of n-grams, tuples of root x note . Downstream task is music segmentation. Metrics are pairwise precision, recall, F1-score. Compared to FORM method, word2vec, fasttext (both on chord symbols), and pitchclass2vec by itself, and concat with word2vec or fasttext. pc2v does highest on over-segmentation (actually looks like under-segmentation: less segments than actually in ground truth/ highest: worse?) and normalized cross entropy. fasttext highest on under-segmentation (actually looks like over-segmentations, more segments than GT/ higher is worse?), pc2vc+ft does best on pairwise F1, fasttext does best on pairwise recall, FORM on simplified chord labels does best on precision.

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

