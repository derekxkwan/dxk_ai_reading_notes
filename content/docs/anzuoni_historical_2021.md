---
title: "A Historical Analysis of Harmonic Progressions Using Chord Embeddings"
date: 2026-02-02T13:45:57-08:00
authors: ["Elia Anzuoni", "Sinan Ayhan", "Federico Dutto", "Andrew McLeod", "Fabian Moss", "Martin Rohrmeier"]
year: 2021
tags: ["embeddings", "representation learning", "hierarchical analysis", "classical music", "musicology", "lstm", "baroque music", "symbolic music", "language-inspired (music)", "early 20th c. (music)", "musicological", "classical period (music)", "roman numeral analysis", "harmonic analysis (music)", "rnn", "music theory", "nlp", "romantic period (music)", "music", "music history", "word2vec"]
categories: ["deep learning", "supervised", "classification", "clustering"]
paper_url: ""
doi: ""
paper_src: "Proceedings of the 18th Sound and Music Computing Conference"
bibkey: "anzuoni_historical_2021"
math: true
draft: false
---

## Summary
Embeds major and minor chord progressions separately from 24 "Western classical composers" from Renaissance to 20th C. with annotations. Given standardization, roman numeral degrees + quality (seventh standardized to triad) forms words in sentences of progressions that are fed to Word2Vec (GenSim) with skip-gram training. Prediction of chords come from embeddings of context chords (window size 2) and results are judged based on accuracy (given that training data is mostly Classical period). Hierarchical clustering (closest link) gives a dendogram of chord embeddings with functionally equivalent (common tones) or functionally different (but close in progression, like V-I) clustered closest in cosine distance. Accuracy highest on major and minor for classical and tapering off in either end, suggesting periods like Renaissance and 20th C don't use chords the same way classical period composers do.

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

