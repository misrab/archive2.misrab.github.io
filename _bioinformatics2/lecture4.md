---
title: Lecture 4 - Prediction of Non-globular Protein Regions
layout: blog
date: 2014-11-10
---

# Bioinformatics II
_Notes from Imperial's Bioinformatics Course_

## Lecture 4 - Prediction of Non-globular Protein Regions

### Intro

Membrane proteins, hey that's a word

Hydrophobic plots, that's a word too!

Homologyyyyy

- MEMSAT3, MEMSAT-SVM, MEMPACK
- TOPCONS (consensus of several methods)
- PHOBIUS


### Signal Peptides

Signal peptides are 15-60 residues at start of protein that direct it to 
correct cellular location.

### Low Complexity Regions

i.e. RRRRRR, RRRSSSRRRRSSS...

Occur in many proteins. Distort stat. significance of alignments.

**SEG** program replaces them with "lowercase" in BLAST???

### Coils

**COILS** program to identify coiled-coils i.e. coiled $$ \alpha $$ helices.

### Disordered Regions of Protein

- PONDR-FIT
- DISOPRED2
- IUPRED

Often proteins become structured only upon docking.