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

- `vcf`: Raw VCF's and other output files from the callers used, currently:

	- MuTect 1.1.4
	- vardict 1.4.6
	- pindel 0.2.5b8

- `maf`: the merged (over the 3 callers), filtered and annotated (VEP) MAF's. Each sample pair (tumor/normal) has its own maf file and there are two maf's

	- standard maf: which has just the events from that sample pair
	- filled-out maf: maf with somatic events and fill-out data from all samples. 

- `qc`: QC-reports and output from the various QC modules run include. There is a master report file: `Proj_<PROJNO>_QC_Report.pdf`
	
- `facets`: Output of facets by running the CMO-facets-suite code:

	https://github.com/mskcc/facets-suite

- `log`: Pipeline log files

