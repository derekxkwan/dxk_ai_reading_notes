---
title: "MUS-ROVER: A Self-Learning System for Musical Compositional Rules"
date: 2026-02-02T13:45:57-08:00
authors: ["Haizi Yu", "Lav Varshney", "Guy Garnett", "Ranjitha Kumar"]
year: 2016
tags: ["generative", "vocal instrumentation", "music", "tsallis entropy", "concept discovery", "bach", "baroque music", "symbolic music", "language-inspired (music)", "handcrafted features", "rule discovery", "music theory", "bach chorales", "classical music"]
categories: ["non-neural network", "probabilistic"]
paper_url: "https://zenodo.org/records/4285220"
doi: "10.5281/zenodo.4285220"
paper_src: "International Workshop on Musical Metacreation (MUME 2016)"
bibkey: "yu_mus-rover_2016"
math: true
draft: false
---

## Summary
Discovers counterpoint/voice leading rules probabilistically from empirical distributions in Bach Chorales. Each vertical alignments represents the GCD of note durations and has chromatic note representations (88 values) for SATB ($88^4$ dimensional vector). Computes probabilistic rules for student (chorale generator) and teacher (adds new probabilistic rule each iteration). Rules are a representation of the vector in a feature space (intervals, pitch classes, note orders, etc.). Computes rules for n-grams (where $n > 1$ grams are conditional probabilities and built upon $n-1$ gram rules). Given sequential learning of rules, offers "chapters" of rules. Defines measures of rule traces called "efficiency" and "memorability"

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

