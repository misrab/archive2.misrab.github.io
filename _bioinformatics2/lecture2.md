---
title: Lecture 2 - Sequence Analysis
layout: blog
date: 2014-11-10
---

# Bioinformatics II
_Notes from Imperial's Bioinformatics Course_

## Lecture 2 - Sequence Analysis

**Paralogues**: gene duplicated, one free to change
**Orthologues**: speciation, then two species have a same gene

### Alignment

- Needleman-Wunsch: find the best _global_ alignment
- Smith-Waterman: instead of looking at sequence in its entirety,
compares segments of all possible lengths

![]({{ site.url }}/images/bioinformatics2/lecture2/1.png)

- BLAST: 50x faster
- PSI-BLAST: Position Specific Iterated i.e. using hits from a BLAST search
- p-values, ROC curves
- Alignment charts:

![]({{ site.url }}/images/bioinformatics2/lecture2/2.png)

- **Multiple alignment**: CLUSTAL family of algorithms. Construct pairwise tree:

![]({{ site.url }}/images/bioinformatics2/lecture2/3.png)

- PROSITE patterns and database: i.e. \[AGT\]{AF}x(n) = or, not, concat n times