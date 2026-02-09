---
title: "Chord Types and Figuration: A Bayesian Learning Model of Extended Chord Profiles"
date: 2026-02-02T13:45:57-08:00
authors: ["Christoph Finkensiep", "Petter Ericson", "Sebasian Klassmann", "Martin Rohrmeier"]
year: 2025
tags: ["harmonic analysis (music)", "music", "variational inference", "jazz", "musicological", "classical music", "instrumental orchestration", "chord profile (music)", "corpus study", "symbolic music", "latent", "music theory", "lead sheet (music)", "elbo", "bayesian", "chord/tone profile (music)", "tone profile (music)"]
categories: ["classification", "supervised"]
paper_url: "https://doi.org/10.1177/20592043241291661"
doi: "10.1177/20592043241291661"
paper_src: "Music & Science"
bibkey: "finkensiep_chord_2025"
math: true
draft: false
---

## Summary
Models a Bayesian model with observed variables being notes and latent variables being chord prototypes and profiles where margianl posteriors (probabilities conditioned on data) can be through variational inference
(stochastic gradient descent on ELBO). Parameters learned are $\theta\_h \in (0,1)$ (chord tone or figuration: beta distribution), $\phi\_{h}^{ct} \in \mathbb{R}^{29}$ (tone-profile vector for chord tones: Dirichlet dist) and  $\phi\_{h}^{ft} \in \mathbb{R}^{29}$ (tone-profile vector for figuration tones: Dirichlet dist). Posterior distributions for tone-profile vectors are studied for differences between models trained on ABC+ (classical music) and EWLD (laed sheets). Mostly similar but ABC+ has more figuration prob (due to chord-scale theory for lead sheets) but EWLD has more ambuiguity in what is chord tone and what is figuration (due to melodies). Dominant chords tend to have more figuration (cadential, longer). EWLD has more enharmonic equivalences (treats dim chords enharmonics as same so all chord tones equal prob). Training is done inferring what is chord tone and what is figuration by figuration having neighbors whole-step at most away which are chord tones.

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

