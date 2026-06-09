# RB-TnSeq analysis notes

This repository contains scripts and documentation from a graduate school RB-TnSeq (Random Barcode Transposon Sequencing) project using a mutant pool of the methylotroph *Methylotenera* sp. JLW8 in planktonic co-culture experiments with the methanotroph *Methylomonas* sp. LW13.

The repository is maintained as an archive of the analysis workflow used for BarSeq count processing, exploratory data analysis, and gene fitness estimation. Raw sequencing data, count tables, and metadata are not included. Scripts are preserved primarily for reference and may require modification before reuse.

## Repository contents

```
data_exploration.Rmd
    Exploratory analysis of BarSeq gene count data, including
    quality control, clustering, PCA, heatmaps, and DESeq2-based
    differential abundance analyses.

FEBA.R
    Main RB-TnSeq gene fitness analysis workflow.

FEBA/
    Experiment-specific FEBA analyses for individual datasets.

loop.sh
    Shell script used during secondary barcode demultiplexing.

demultiplexing_strategy.md
    Documentation of the dual-index BarSeq library design,
    barcode structure, demultiplexing workflow, and required
    software tools.

README.md
    Repository documentation.
```

## General workflow

1. Demultiplex sequencing reads (loop.sh)
2. Generate gene count table
3. Explore count data (data_exploration.Rmd)
4. Estimate gene fitness (FEBA.R)

## Data availability

Raw sequencing reads, count tables, and metadata are not included in this repository. File paths in the scripts reflect the original local or cluster environment and may need to be modified before reuse.
