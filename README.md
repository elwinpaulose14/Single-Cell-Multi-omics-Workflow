# Single-Cell-Multi-omics-Workflow
This workflow represents analysis of single-cell RNA and ADT data by employing Seurat in R. This analysis provides a complete picture from loading your .rds file to multi-omic profiling. 


# Overview

This pipeline enables preprocessing, quality control, dimensionality reduction, trajectory analysis, gene set enrichment analysis (GSEA), and integration of single-cell RNA/ADT data with a reference bone marrow dataset using Symphony.

# Installation

Install required R packages via [Bioconductor](https://bioconductor.org/) and devtools

# Data Preparation

- Place your RNA Seurat object and Sample Tag calls (`.rds` and `.csv`) in the appropriate folder.
- Download reference objects for Bone Marrow Map via the provided URLs.

# Workflow Steps

1. Load Data  
   - Load RNA data and sample metadata.
2. Preprocessing  
   - Filter cells, calculate mitochondrial percentage, and normalize data.
3. Subgrouping & Normalization  
   - Subset cells by sample tag and normalize ADT and RNA assays.
4. Dimensionality Reduction  
   - Run PCA, UMAP, and clustering.
5. Annotation  
   - Add metadata and visualize clusters.
6. Bone Marrow Map Integration  
   - Project your data onto the bone marrow reference using Symphony.
7. Trajectory Analysis  
   - Perform pseudotime and trajectory inference using Monocle3.
8. GSEA  
   - Run gene set enrichment analysis on normalized expression profiles.
9. Multi-omics Visualization  
   - Compare RNA and ADT features across clusters.

# Integration with Bone Marrow Map

The workflow leverages the `BoneMarrowMap` and `Symphony` for mapping your dataset onto a curated reference, facilitating cell type annotation and trajectory analysis.

# Results & Visualization

# Example Preprocessing Plot



# Multi-omics Profile


# Symphony Integration





## References

- [Seurat Documentation](https://satijalab.org/seurat/)
- [BoneMarrowMap Package](https://github.com/dosorio/boneMarrowMap)
- [Symphony Reference Mapping](https://cran.r-project.org/web/packages/symphony/index.html)

---

## Contact

For questions, open an issue or contact [@elwinpaulose14](https://github.com/elwinpaulose14).
