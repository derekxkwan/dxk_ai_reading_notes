---
title: "Relevance of musical features for cadence detection"
date: 2026-02-02T13:45:57-08:00
authors: ["Louis Bigo", "Laurent Feisthauer", "Mathieu Giraud", "Florence Levé"]
year: 2018
tags: ["harmonic analysis (music)", "music", "svm", "instrumental orchestration", "cadence detection (music)", "classical period (music)", "baroque music", "symbolic music", "handcrafted features", "music theory", "classical music"]
categories: ["non-neural network", "supervised"]
paper_url: "https://hal.science/hal-01801060"
doi: ""
paper_src: "International Society for Music Information Retrieval Conference (ISMIR 2018)"
bibkey: "bigo_relevance_2018"
math: true
draft: false
---

## Summary
Describes handcrafted features (Boolean) to extract from symbolic representations (datasets: bach-wtc-i and haydn-quartets with annotations). Describes cadences with chords X,Y,Z in order (Z being the last chord) and features such as type of chord (Z-in-perfect triad) or note composition, voice leadings from Y-to-Z (with note degrees with relation to bass note) and X-to-Y as well as rests after Z, if chords are on downbeats, etc. Represented as binary vectors and trained using SVM with wextra weights on cadential beats using leave-one-piece-out cross val. 75\% acc on PAC with low false positives, 50\% on HC (half cadences). Combining rIAC (rooted imperfect authentic cadence with the IAC in root position) with PAC drops accuracy to 68\% on Bach WTC.

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

