# RNA_Seq_Clustering

# RNA-Seq Clustering and Visualization

This project demonstrates the analysis, clustering, and visualization of single-cell RNA sequencing (scRNA-seq) data. It utilizes the PBMC 3k dataset provided by Scanpy, performing key steps such as data preprocessing, dimensionality reduction, clustering, and marker gene identification. The results include a UMAP visualization of identified clusters and annotations of cell types.

## Features

- **Data Preprocessing:** Filters low-quality cells and genes, normalizes the data, and identifies highly variable genes.
- **Dimensionality Reduction:** Applies Principal Component Analysis (PCA) to reduce data dimensions.
- **Clustering:** Constructs a KNN graph and uses the Leiden algorithm for clustering.
- **Visualization:** Uses UMAP for visualizing clusters and their annotations.
- **Marker Gene Identification:** Identifies top marker genes for specific clusters.
- **Annotation:** Assigns biological cell type labels to clusters.

## Prerequisites

- Python 3.7+
- Required Python libraries:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `scikit-learn`
  - `umap-learn`
  - `leidenalg`
  - `igraph`
  - `scipy`
  - `scanpy`

Install the dependencies using pip:
```bash
pip install pandas numpy matplotlib scikit-learn umap-learn leidenalg igraph scipy scanpy
```

## Usage

1. Clone the repository and navigate to the project directory.
2. Run the Python script or Jupyter notebook.
3. The script will:
   - Load the PBMC 3k dataset.
   - Preprocess the data (filter, normalize, transform).
   - Perform PCA for dimensionality reduction.
   - Cluster the data using the Leiden algorithm.
   - Visualize the clusters with UMAP.
   - Identify marker genes for clusters.
   - Save annotated results to `annotated_results.csv`.

## Visualizations

- **PCA Explained Variance:**
  Displays the cumulative variance explained by the principal components.

- **UMAP Clusters:**
  Visualizes clusters in 2D space, colored by cluster ID.

- **UMAP with Cell Type Annotations:**
  Visualizes clusters with cell type labels assigned to each cluster.

## Outputs

- **annotated_results.csv:**
  A CSV file containing UMAP coordinates, cluster IDs, and annotated cell types.

## Example Results

### Top Marker Genes
Example output:
```
Top marker genes for Cluster 0: ['GeneA', 'GeneB', 'GeneC', ...]
```

### UMAP Visualization
- A scatter plot showing clusters in reduced dimensions.
- Annotated cell types overlayed on the UMAP visualization.
Feel free to contribute or modify the script to adapt it for other scRNA-seq datasets or analysis needs!
