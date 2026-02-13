---
title: "deepGTTM-III: Multi-task Learning with Grouping and Metrical Structures"
date: 2026-02-13T10:52:18-08:00
authors: ["Masatoshi Hamanaka", "Keiji Hirata","Satoshi Tojo"]
year: 2018
tags: ["gttm", "music analysis", "hierarchical music analysis", "music segmentation", "symbolic music", "deep belief network"]
categories: ["deep learning", "probabilistic", "multi-task"]
paper_url: ""
doi: ""
paper_src: "Music Technology with Swing"
bibkey: "hamanaka2018"
math: true
draft: false
---

## Summary
This paper essentially stithes together deepGTTM-I and deepGTTM-II together to form deepGTTM-III (as the group boundaries of -I interact with the metrical boundaries of -II). Some additional detail is given on GPRs and MPRs. deepGTTM-III takes the input format of deepGTTM-I and has outputs corresponding to deepGTTM-I and -II. The additional input of group boundaries for deepGTTM-II is unneeeded as now -I and -II are merged as one model. Outperforms -I but -II has slightly higher performance (-II has ground truth boundaries).

## Key Contributions
Merge deepGTTM-I and -II together to form -III to be able to deal with interactions between GTTM group and metrical boundaries.

## Limitations and Future Work


## Key Equations


## Other Notes
