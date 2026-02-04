---
title: "Identifying Irish Traditional Music Genres Using Latent Audio Representations"
date: 2026-02-02T13:45:57-08:00
authors: ["Diego M. Jiménez-Bravo", "Álvaro Lozano Murciego", "Juan José Navarro-Cáceres", "María Navarro-Cáceres", "Treasa Harkin"]
year: 2024
tags: ["mule", "musicology", "music theory", "melodic (music)", "lda", "genre classification (music)", "vocal instrumentation", "midi", "mert", "irish", "jukebox", "music", "musicxml", "symbolic music", "representation leveraging", "symbolic music to audio", "folk music"]
categories: ["supervised", "non-neural network", "classification"]
paper_url: "https://ieeexplore.ieee.org/abstract/document/10579819"
doi: "10.1109/ACCESS.2024.3421639"
paper_src: "IEEE Access"
bibkey: "jimenez-bravo_identifying_2024"
math: true
draft: false
---

## Summary
Classify types of Irish folk music obtained from ITMA and the The Session. Files are MusicXML and then process is to convert to MIDI and render as WAV and then feed into MERT, Jukebox, and MULE and extract activations. Apply various classification algos to activations from PyCaret and scikit-learn (LDA, ridge classifier, MLP, random forest, extra trees, logistic regression, SVM with linear kernel, KNN, decision trees, naive bayes, quadratic discriminant analysis). Results not "great" according to authors but best was Jukebox with LDA (85\%) with poor performance blamed on synthesized vs real instruments as well as everything being dancy.

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

