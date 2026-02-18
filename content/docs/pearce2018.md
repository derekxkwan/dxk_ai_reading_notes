---
title: "Statistical learning and probabilistic prediction in music cognition: mechanisms of stylistic enculturation"
date: 2026-02-18T01:40:02-08:00
authors: ["Marcus T. Pearce"]
year: 2018
tags: ["music perception", "statistical learning", "probabilistic prediction", "symbolic music", "music", "music theory", "monophonic"]
categories: ["unsupervised", "probabilistic"]
paper_url: ""
doi: "10.1111/nyas.13654"
paper_src: "Annals of the New York Academy of Sciences"
bibkey: "pearce2018"
math: true
draft: false
---

## Summary
Discusses the IDyOM model that is a "variable-order Markov model" that models probabilities of aspects of note events (pitch, onset time, inter-onset interval, ioi ratio, scale degree, pitch interval, etc.) in monophonic music. Composed of long-term (to simulate listener previous exposure to music) and short-term (to simulate present listening experience) models. Aspects can be measured in conjunction (namely, pitch and time aspects), denoted by $\otimes$.

Based on the statistical learning hypothesis (listener statistical models of music acquired from exposure) and the probabilistic prediction hypothesis (application of SLH to currently encountered music to predict what happens next).

Empirically shown to have ties to "expectation, emotional response, recognition memory, phrase boundary perception, perceptual similarity, and meter perception" (given adjustments for meter perception which is a Bayesian model for predicting meter with prior for meter and likelihood of note onsets given meter). Using the long-term model, shown to model exposure to a different music culture than a listener's own (Chinese vs Western folk songs).

## Key Contributions
Probabilistic model that measures information concent and entropy of note events in monophonic music for a listener. 

## Limitations and Future Work
Model listener familiarity with multiple cultures of music. Extension to polyphonic music. Extention to "musical cultures that have no written tradition" (audio?). Study of effects of musical training on perception. 

## Key Equations
entropy: $H = - \sum_{p \in P} p \log p$

information content: $h = -\log_{10} p$

## Other Notes
