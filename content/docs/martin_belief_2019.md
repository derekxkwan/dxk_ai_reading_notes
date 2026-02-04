---
title: "Belief Propagation algorithm for Automatic Chord Estimation"
date: 2026-02-02T13:45:57-08:00
authors: ["P. Vincent Martin", "Sylvain Reynal", "Dogac Basaran", "Hélène C. Crayencour"]
year: 2019
tags: ["no training", "music theory", "structure annotation (music)", "hmm", "hidden markov", "popular music", "chroma", "automatic chord estimation", "music", "belief propagation", "bayesian", "audio", "beatles"]
categories: ["non-neural network", "probabilistic"]
paper_url: "https://hal.science/hal-02132416"
doi: ""
paper_src: "16th Sound & Music Computing Conference"
bibkey: "martin_belief_2019"
math: true
draft: false
---

## Summary
functions (original goes between bars; prime goes between beats in bars in mod 1,2 steps; double prime between same beat in phrases).  Uses max-sum variant of BP and can use phrase structure annotation as well as ground truth or estimated downbeats. Can also optionally use Foote's SSM but not better results. BP beats HMM variance in all cases (except using perceptual transition matrix from Krumhansl). BP with downbeats and structure annotation best (slightly less with cycle of fifths transitions and correlation variants with both). Does not beat SOTA. Run on Beatles subset of Isophonics.

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

