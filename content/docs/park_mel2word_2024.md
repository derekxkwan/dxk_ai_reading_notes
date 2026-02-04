---
title: "Mel2Word: A Text-Based Melody Representation for Symbolic Music Analysis"
date: 2026-02-02T13:45:57-08:00
authors: ["Saebyul Park", "Eunjin Choi", "Jeounghoon Kim", "Juhan Nam"]
year: 2024
tags: ["handcrafted features", "melodic (music)", "music theory", "genre classification (music)", "nlp", "inter-onset interval (music)", "representation learning", "segmentation", "bpe", "music", "symbolic music", "language-inspired (music)", "folk music"]
categories: ["non-neural network"]
paper_url: "https://doi.org/10.1177/20592043231216254"
doi: "10.1177/20592043231216254"
paper_src: "Music & Science"
bibkey: "park_mel2word_2024"
math: true
draft: false
---

## Summary
Using MTC-ANN dataset (Meertens Tune Collection with annotations), learns embeddings of melodies through encoding them into letters and numbers (intervals, quantized inter-onset intervals in notes) and learns a segmenting process through BPE, which are then tokenized. With the downstream task of  tune families, bigger dictionary size means higher performance (up to a point). Using just pitch features better than just rhythm, both together slightly better than just pitch. Performs better than other segmentation algs (morphere, markov, 2-gram, LBDM, GPR, Gestalt, 3-gram) with smaller dictionary size.

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

