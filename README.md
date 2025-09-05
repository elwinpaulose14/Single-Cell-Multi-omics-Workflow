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





# Preprocessing Plot
<img width="1902" height="870" alt="image" src="https://github.com/user-attachments/assets/540278d2-b749-4608-9996-541b8e481b4b" />


# Symphony Integration
<img width="1789" height="901" alt="image" src="https://github.com/user-attachments/assets/3c1b6f74-4eaf-48f5-9da6-159c9f2a1b93" />


# Multi-omics Profile
<img width="1902" height="865" alt="image" src="https://github.com/user-attachments/assets/d61e2062-233a-4d01-8afc-c8b5b033883f" />








## References
- Seurat Package(https://satijalab.org/seurat/)
- Symphony Reference Mapping(https://cran.r-project.org/web/packages/symphony/index.html)
- Zeng AGX, Iacobucci I, Shah S, Mitchell A, Wong G, Bansal S, Chen D, Gao Q, Kim H, Kennedy JA, Arruda A, Minden MD, Haferlach T, Mullighan CG, Dick JE. 
Single-cell transcriptional mapping reveals genetic and non-genetic determinants of aberrant differentiation in AML. 
*Nature Genetics*. 2022. https://doi.org/10.1038/s41588-022-01043-0

---

## Contact

For questions, open an issue or contact [@elwinpaulose14](https://github.com/elwinpaulose14).
