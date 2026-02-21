# Multi-omics-MachineLearning-in-IPF

This repository contains R scripts for bulk transcriptomics analysis, WGCNA, single-cell transcriptomics, and machine-learning modeling in idiopathic pulmonary fibrosis (IPF).

## Code structure

- **Analysis.GSE32537+GSE110147.R**  
  Bulk GEO data analysis script for IPF/control cohorts (data loading, basic preprocessing, and differential expression outputs).

- **Analysis.WGCNA.R**  
  WGCNA pipeline for identifying co-expression modules and relating modules to clinical traits.

- **Analysis.Single-cell.Transcriptomic.R**  
  Single-cell RNA-seq analysis workflow (Seurat-based processing, integration/clustering, and cell-type annotation).

- **pipline.Machine.learning.R**  
  Core machine-learning function library (model training utilities, feature handling, prediction, and evaluation helpers).  
  This file is intended to be sourced by other ML scripts.

- **Output.Machine.learning.R**  
  End-to-end machine-learning run script that uses the pipeline functions to train models and generate prediction/performance outputs.

## Notes
- Scripts are designed to be run independently, depending on which analysis you need (bulk, WGCNA, scRNA-seq, or ML).
- Update file paths at the top of each script to match your local data location.
