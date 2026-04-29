# B528_GEETHANJALI_KARUTURI_project_2026

## Multi-Omics Integration of Single-Cell RNA and ATAC Sequencing via Fused Gromov-Wasserstein Optimal Transport

Cross-modal integration of snRNA-seq and snATAC-seq using Fused Gromov–Wasserstein (FGW) optimal transport with GRN analysis in human myocardial tissue.

---

## Overview
This project integrates unpaired single-nucleus RNA-seq (snRNA-seq) and single-nucleus ATAC-seq (snATAC-seq) data using FGW optimal transport. The goal is to recover biologically meaningful correspondences and construct gene regulatory networks (GRNs) in human myocardium.

---

## Objectives
- Integrate unpaired snRNA-seq and snATAC-seq datasets  
- Preserve intra-modal geometry and align cross-modal features  
- Evaluate alignment using Pearson correlation coefficient (PCC)  
- Construct component-level gene regulatory networks  

---

## Methods
- **Preprocessing:** Normalization (10,000 counts) and log transformation using Scanpy  
- **Feature Selection:** 5,000 highly variable genes (Seurat method)  
- **Dimensionality Reduction:** PCA (50 components, ARPACK solver)  
- **Integration:** FGW optimal transport using POT  
- **Post-alignment:** Barycentric projection and variance rescaling  
- **Evaluation:** Mean PCC vs random baseline  
- **GRN Construction:** Correlation-based network using NetworkX  

---

## Data Sources
- CELLxGENE (scRNA-seq and scATAC-seq datasets)  
- Zenodo (additional datasets)  

*Note: Raw datasets are not included due to size. Please download from the original sources.*

---

## Results
- FGW achieved higher cross-modal PCC than a random baseline  
- Hub components correspond to known cardiac cell types  
- GRN captures biologically meaningful regulatory programs  

---

## Key Libraries
- Scanpy  
- scikit-learn  
- Python Optimal Transport (POT)  
- NetworkX  
- NumPy  
- Pandas  

---
## Acknowledgments
This project benefited from the use of ChatGPT for assistance with organization and structuring of content, and Grammarly for improving clarity and sentence formulation.
