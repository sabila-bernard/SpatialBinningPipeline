# SpatialBANKSY
Curio Seeker spatial transcriptomics data are high-dimensional and sparse, resulting in low signal-to-noise ratios for downstream analyses. To address this, this pipeline performs spatial binning of Curio Seeker data into grids, improving UMI counts while preserving spatial structure. 

The binned data are then processed with BANKSY ([GitHub](https://github.com/prabhakarlab/Banksy/blob/devel/README.md)), a neighborhood-based analysis method, that integrates each bin's gene expression with that of its neighbors. BANKSY accounts for spatial relationships and context between each bins and enables the identification of coherent spatial domains.

# Getting Started 
The pipeline requires the packages listed below:
```
library(Seurat)
library(sf)
library(dplyr)
library(ggplot2)
library(patchwork)
library(SeuratData)
library(dbscan)
library(pheatmap)
library(clustree)
library(dplyr)
library(purrr)
library(clusterProfiler)
library(org.Mm.eg.db)
library(SeuratWrappers)
library(Banksy)
library(clusterProfiler)
```

