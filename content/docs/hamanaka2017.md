---
title: "deepGTTM-I&II: Local Boundary and Metrical Structure Analyzer Based on Deep Learning Technique"
date: 2026-02-12T21:59:48-08:00
authors: ["Masatoshi Hamanaka", "Keiji Hirata","Satoshi Tojo"]
year: 2017
tags: ["gttm", "music analysis", "hierarchical music analysis", "music segmentation", "symbolic music" "pcfg", "probabilistic context-free grammar", "deep belief network"]
categories: ["deep learning", "probabilistic", "multi-task"]
paper_url: ""
doi: ""
paper_src: "Bridging People and Sound"
bibkey: "hamanaka2017"
math: true
draft: false
---

## Summary
Learns a DBN for "local grouping boundaries" (deepGTTM-I) corresponding to grouping preference rules (GPR) 2a, 2b, 3a, 3b, 3c, 4, 5, 6, 7 of the GTTM. Learns a "metrical structure (deepGTTM-II) corresponding to metrical preference rules (MPR) 2, 3, 4, 5a, 5b, 5c, and 5d. Inputs of both are "onset" and "offset time, pitch, and velocity". from musicXML. deepGTTM-II takes in annotated "grouping structure". Outputs are application of rule or strong beat (1) and non-application or weak beat (0). Trained on GTTM database, music annotated by automatic time-span tree analyzer (ATTA), and "300 pieces of 8-bar-long, monophonic, classical music" hand-annotated.

## Key Contributions
Deep belief networks trained to output GPRs and MPRs of GTTM for grouping and metrical structure. New dataset annotated by musicologists.

## Limitations and Future Work
Generation of "time-span and prolongation tree structures".

## Key Equations


## Other Notes
