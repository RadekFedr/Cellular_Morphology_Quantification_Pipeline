# Cellular Morphology Quantification Pipeline

## Overview

This project is designed to analyze **morphological features of cellular data**, focusing on nucleus and cell parameters such as intensity, area, perimeter, and shape. The pipeline calculates key statistics, generates PDF report with visualizations, applied clustering and dimensionality reduction techniques to explore the data.

On the pipeline's input should be raw images from the Olympus FV10i confocal microscope. 

One-click script compares different morphology phenotypes of **one repetition** experiment. It was designed for comparison up to **20 different samples** (cell lines, conditions, clones).

The pipeline outputs summary statistics, visual plots, heatmaps, and dimensionally reduced representations (PCA, t-SNE, UMAP) of the data. Results are exported in various formats, including Excel, CSV, and PNG.

## Features
- **Statistics Calculation**: Computes the mean and standard deviation of cellular features across different groups.
- **Visualizations**: Produces violin, boxplots for morphological parameters.
- **Clustering**: Performs hierarchical clustering of groups and generates a heatmap of the results.
- **Dimensionality Reduction**: Applies PCA, t-SNE, and UMAP to visualize data structure in reduced dimensions.
- **Object-level Analysis**: Includes detailed object-level output for further exploration.

## Outputs
The pipeline generates the following outputs:

- **PDF report** , detailed summary of results provided to the user.
- **Excel files** containing summary statistics of cell and nucleus parameters for each group.
- **PNG images** of violin/boxplots for parameter comparison, heatmaps, and dimension reduction plots.
- **CSV files** with PCA, t-SNE, and UMAP results for each object.

## Usage
The pipeline is built using `R` and requires appropriate packages for data manipulation, plotting, and clustering, including:

- `ggplot2`
- `dplyr`
- `Rtsne`
- `umap`
- `pheatmap`
- `openxlsx`

Ensure that the data is structured properly and loaded into the pipeline for correct analysis.

## License
This project was built as a demonstration of skills and a personal portfolio and is licensed for non-commercial use only. You are not permitted to copy, modify, or distribute the code for commercial purposes without explicit permission from the author.

© Radek Fedr, 2024. All rights reserved.

---

This is a high-level overview of the pipeline's functionality. Please refer to the source code and function documentation for more details.