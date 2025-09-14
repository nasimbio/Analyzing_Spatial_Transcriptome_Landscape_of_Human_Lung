# Analyzing Spatial Transcriptome Landscape of Human Lung

This project analyzes high-resolution spatial transcriptomics data from human lung tissue using the 10x Genomics **Visium HD** platform. The goal is to perform unsupervised clustering, anatomical region annotation, and spot-level cell type deconvolution using a well-annotated external single-cell RNA-seq reference.

---

## 📘 Project Overview

Spatial transcriptomic profiling of human lung tissue was performed using the **Visium HD** platform, which offers subcellular resolution. Standard preprocessing, dimensionality reduction, and clustering were conducted to capture spatial gene expression patterns and identify distinct tissue regions.  
To resolve the cellular composition of each spatial location, I employed the **RCTD** algorithm, leveraging an external single-cell reference atlas for robust deconvolution of Visium HD spots.

---

## 📊 Analysis Tasks

### **Task 1: Preprocessing, Clustering, and Regional Annotation**
- Normalize the Visium HD spatial dataset
- Apply **sketching** for dimensionality reduction on a subset of the data
- Perform **PCA** and **clustering** on the sketch, then project results to the full dataset
- Visualize clustering results using UMAP and spatial plots
- Conduct **BANSKY** analysis to define anatomical regions of the lung tissue

### **Task 2: Cell Type Deconvolution via RCTD**
- Prepare a well-annotated single-cell reference dataset
- Normalize and format the reference expression and metadata
- Construct an **RCTD reference object**
- Process the Visium HD query dataset into a compatible RCTD spatial object
- Run the **RCTD algorithm** to infer cell type composition at each spot
- Visualize deconvolution results to interpret spatial cell type distribution

---


# 💡 Notes

- Raw data is not publicly available due to client ownership and confidentiality.
- Some example outputs plots are organized by task in the `output/` folder.
- This project is designed for both reproducibility and clarity.

---

## 📬 Contact

*Author:* Nasim Rahmatpour 
*Email:* nasimrahmatpour1@gmail.com 
*GitHub:* (https://github.com/nasimbio)

