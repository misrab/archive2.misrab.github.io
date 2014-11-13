---
title: Lecture 0 - Jargon
layout: blog
date: 2014-11-09
---

# Bioinformatics II
_Notes from Imperial's Bioinformatics Course_

## Lecture 0 - Jargon

### Misc

- NCBI (USA), EBI (UK): bioinformatics institutes

### Protein Folding

- Protein Data Bank (PDB) (managed by RCSB, EBI...)
- SCOP, CATH classifications in PDB. SCOP below: 

![]({{ site.url }}/images/bioinformatics2/lecture0/1.png)

![]({{ site.url }}/images/bioinformatics2/lecture0/2.png)

Families manually constructed.

SCOP2 being developed with more complex hierarchy.

CATH:

![]({{ site.url }}/images/bioinformatics2/lecture0/3.png)

### Sequence Analysis

- INSDC (International Nucleot. Seq. Db Collection)
- GenBank in USA
- EBML (European Mol Bio Lab)
- DDBJ (Japan)
- SWISSPROT high quality manual annotation

### Algorithms

- PAM (point accepted mutation). PAM250 scoring matrix:

![]({{ site.url }}/images/bioinformatics2/lecture0/4.png)

- BLOSUM: (BLock SUb Matrix). Just a different matrix.
- FASTA (old), BLAST
- PSI-BLAST: Position Specific Iterated i.e. using hits from a BLAST search
- PROSITE patterns and database: i.e. \[AGT\]{AF}x(n) = or, not, concat n times

