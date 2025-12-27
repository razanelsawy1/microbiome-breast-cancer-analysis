# microbiome-breast-cancer-analysis
Gut microbiome analysis pipe# Gut Microbiome Analysis in Breast Cancer

## Project Overview
This project explores differences in gut microbiome composition between
breast cancer patients and healthy controls using 16S rRNA sequencing data.
The analysis follows a standard QIIME 2 microbiome workflow, including data
download, quality control, denoising, taxonomic profiling, and diversity analysis.

## Dataset
- Source: NCBI Sequence Read Archive (SRA)
- Data type: Paired-end 16S rRNA sequencing
- Number of samples: 52
- Accession numbers are listed in `data/srr_accessions.txt`

## Pipeline Summary
The intended analysis pipeline consists of the following steps:

1. Download raw sequencing data from SRA using `prefetch` and `fasterq-dump`
2. Perform quality control using FastQC
3. Import paired-end FASTQ files into QIIME 2
4. Denoise sequences using DADA2
5. Assign taxonomy using the SILVA reference database
6. Perform alpha and beta diversity analyses
7. Identify differentially abundant taxa

## Execution Notes
Initial steps including data download, FASTQ generation, and quality assessment
were successfully completed. However, denoising and downstream analyses could
not be fully executed due to hardware and storage limitations on the local system.
The remaining steps are documented as planned commands and reflect standard
QIIME 2 practices.

Example figures representing expected analysis outputs are provided in the
`results/figures` directory for demonstration and interpretation purposes.

## How to Run
The scripts in the `scripts/` directory describe the full analysis workflow.
They can be executed on a system with sufficient computational resources and
a working QIIME 2 installation.

## Tools Used
- QIIME 2 (v2024.2)
- FastQC
- SRA Toolkit (prefetch, fasterq-dump)
- Python (for visualization)
- Galaxy platform (partial execution)

## Author Notes
This repository focuses on reproducibility, workflow clarity, and correct
biological interpretation of microbiome data.
line for breast cancer study
