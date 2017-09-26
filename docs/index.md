---
layout: default
overview: true
title: Roslin Variant Pipeline Output
---

# Roslin Variant Pipeline Output

## Source code for pipeline

- https://github.com/mskcc/prism-pipeline

- Version 1.1 (?)

## Output folder organization

In the output folder you will find one file:

- `Proj_<PROJNO>_request.txt`

which will have the pipeline request manifest file. In additiona there are the following folder: 

- `inputs`: contains the input files used in running the pipeline

- `bam`: bam files that have been: sorted, mark-duplicated, abra-realigned, GATK-baseQ-recalibrated.

- `vcf`

- `maf`

- `qc`

- `facets`

- `log`

`inputs`
