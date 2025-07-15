# E10ScRNAData
# 🧬 E10 scRNA-seq and ATAC-seq Data Analysis

This project focuses on the integrative analysis of **single-cell RNA-sequencing (scRNA-seq)** and **single-cell ATAC-sequencing (scATAC-seq)** data from **E10 mouse embryonic tissues**, with an emphasis on neural crest and neuroepithelial development.

---

## 🧠 Objective

To understand early cell fate specification and chromatin accessibility dynamics at embryonic day 10 (E10) by integrating transcriptomic and epigenomic single-cell data.

---

## 🔍 Data Overview

- **Organism**: Mus musculus (mouse)
- **Developmental Stage**: Embryonic Day 10 (E10)
- **Tissues**: Neural tube, cranial region, mesoderm
- **Modalities**:
  - scRNA-seq: Gene expression profiling
  - scATAC-seq: Chromatin accessibility

---

## 🧪 Methodology

### 🔹 scRNA-seq Pipeline
- Preprocessing with CellRanger or STARsolo
- Quality control with `Seurat`
- Clustering and dimensionality reduction (PCA, UMAP)
- Cell type annotation via known markers
- Differential expression and trajectory inference (`Monocle3`, `scVelo`)

### 🔹 scATAC-seq Pipeline
- Preprocessing with CellRanger-ATAC
- Quality control with `Signac`
- Peak calling and motif analysis
- Gene activity matrix generation
- Pseudo-bulk accessibility and differential peak analysis

### 🔹 Integration
- Anchored integration of scRNA and scATAC with `Seurat v5` + `Signac`
- Co-accessibility analysis (Cicero or `ArchR`)
- Joint visualization of gene expression and accessibility

---

## 📁 Repository Structure

```bash
E10ScRNAandATACseqData/
├── data/                   # Raw and preprocessed input data
├── scripts/                # Analysis scripts (R/Python/Notebooks)
├── results/                # Output figures, tables, and metrics
├── notebooks/              # Annotated analysis workflows
├── figures/                # Publication-ready plots
└── README.md               # This file
