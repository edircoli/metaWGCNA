# metaWGCNA

## Overview
This repository contains the analysis pipeline, data, and source code for the "metaWGCNA" framework: a co-expression analysis of metatranscriptomics to understand organic micropollutants degradation in complex microbiomes. This study applies eWeighted Gene Co-expression Network Analysis (WGCNA) to analyses Metatranscriptomics and Metagenomics in a single-omics and multi-omics perspective at the module level. The main purpose of the analysis is to understand Organic Micropollutant (OMP) degradation rates in wastewater microbiomes.

![metaWGCNA Framework](images/illustrations/metaWGCNA.png)

## Objectives
1.  **Metatranscriptomics WGCNA:** Identify co-expression modules from the taxonomic groups and correlate them with OMP degradation rates (kbios).
2.  **Metagenomics WGCNA:** Analyze taxonomic abundance co-occurrence modules and correlate them with OMP degradation.
3.  **Cross-Omics Integration:** Correlate eigengenes from transcript modules with taxonomic modules.
4.  **Functional Enrichment:** Perform enrichment analysis (KEGG/NOGs) for modules significantly correlated with degradation.

## Repository structure

metaWGCNA/
├── analysis.Rmd 
├── data/
│   ├── raw_counts/
│   │   └── 2024-10-01_spades_transcript_counts.csv
│   ├── metadata/
│   │   ├── clusters.tsv
│   │   ├── coverm_drep-relative_abundances.tsv
│   │   └── nitrosomonas_kbios.csv
│   └── enrichment/
│       ├── gtdbtk.bac120.summary.tsv
│       └── out.bin.all.emapper.annotations.zip <-- (Uncompressed for analysis)
├── images/
│   ├── illustrations/
│   └── results/    
└── README.md