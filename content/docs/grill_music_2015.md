---
title: "Music Boundary Detection Using Neural Networks on Combined Features and Two-Level Annotations."
date: 2026-02-02T13:45:57-08:00
authors: ["Thomas Grill", "Jan Schlüter"]
year: 2015
tags: ["convolutional", "music boundary", "hierarchical analysis", "hpss", "music", "audio", "self-similarity matrix", "log mel spectrogram", "cnn", "representation learning", "non-bar/beat aligned similarity", "multi-level", "segmentation", "multi-representation", "music theory", "boundary detection (music)", "log-mel spectrogram"]
categories: ["deep learning", "supervised"]
paper_url: "https://zenodo.org/records/1417461"
doi: "10.5281/zenodo.1417461"
paper_src: ""
bibkey: "grill_music_2015"
math: true
draft: false
---

## Summary
Uses training format of ullrich\_boundary\_2014 to train CNN features with log-Mel and log-Mel harmonic-percussive source separation. Calculates both SSM and SSM with concatenate features in windows (looping around in case of negative time steps). cosine-similarity is soft thresholded. Uses SALAMI. Performs best with all features on tolerance of $\pm 0.5$ seconds compared to MIREX 2012 to 2014 on first and second level boundaries (SALAMI has two levels of annotations).

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

