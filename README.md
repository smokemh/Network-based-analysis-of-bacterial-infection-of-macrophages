# Network-based-analysis-of-bacterial-infection-of-macrophages

## Overview

This repository documents a comprehensive network-based analysis of bacterial infection in macrophages, focusing on Legionella pneumophila. The project aims to construct a core regulatory network of genes active in macrophages post-infection.

## Project Description

Macrophages (Mphs) are key immune cells that coordinate the immune response against infections. This project utilizes transcriptomics datasets from human primary Mphs infected with Legionella pneumophila to analyze healthy and affected genes. The methodology involves programming in R language for data organization, normalization, differential expression analysis, and visualization using various plots and graphs. Additionally, network analysis algorithms are applied to identify a core regulatory
network.

### 1. Dataset Acquisition

- Obtained datasets from GEO (Legionella pneumophila: GSE61535), focusing on the 3 uninfected and 3 wild-type infected human primary Mphs replicates.
- Pre-processed and log-transformed data.

### 2. Differential Expression Analysis

- Performed differential expression analysis comparing control to infection.
- Corrected p-values and produce visualizations, such as volcano plots, MD plot and PCA.

### 3. Feature Selection and Pathway Enrichment

- Applied feature selection procedures to identify the top 100 most relevant genes.
- Generate a heatmap for the selected genes and conduct pathway enrichment analysis.

### 4. Network Analysis

- Utilized existing computational tools and databases like Cytoscape, String, and Reactome.
- [Cytoscape](https://cytoscape.org/): For visualizing and merging networks, as well as executing network biology algorithms.
- [String](https://string-db.org/): A database of protein-protein interactions useful for building networks.
- [Reactome](https://reactome.org/): A curated pathways database.

- Explored interactions connecting differentially expressed genes.
- Apply network analysis algorithms to unveil a core regulatory network.

### 5. Drug Target Exploration

- Investigated drugs targeting genes in the core network.
- Predicted the potential effects of these drugs within the network.

## Running the Project in R Studio

### Prerequisites

- Install R: [Download R](https://cran.r-project.org/)
- Install R Studio: [Download R Studio](https://rstudio.com/products/rstudio/download/)

### Clone Repository

Clone this repository to your local machine:

````bash
git clone https://github.com/smokemh/Network-based-analysis-of-bacterial-infection-of-macrophages

### Set Up R Studio Workspace
- Open R Studio.
- Navigate to File -> Open Project.
- Select the cloned repository directory.

### Required R Libraries

- `GEOquery`: Used for accessing and retrieving Gene Expression Omnibus (GEO) data.
- `dplyr`: Provides a set of tools for efficiently manipulating data frames.
- `pheatmap`: Enables the creation of interactive heatmaps for gene expression analysis.
- `ggplot2`: A versatile package for creating visually appealing plots and graphs.
- `ggrepel`: Adds functionality to 'ggplot2' for avoiding overplotting of text labels.
- `readr`: Used for reading and writing structured text data.
- `limma`: Employs linear models for microarray data analysis.
- `org.Hs.eg.db`: Provides a set of annotation maps for human genes.
- `tidyverse`: A collection of R packages for data manipulation and visualization.
- `enrichR`: Used for gene set enrichment analysis.
- `pathview`: Allows visualization of biological pathways.
- `org.Mm.eg.db`: Provides annotation maps for mouse genes.
- `EBImage`: Offers image processing tools for biological images.

### Install Required Packages

In the R Studio console, run the following commands to install the required packages:

```R
install.packages("GEOquery")
install.packages("dplyr")
install.packages("pheatmap")
install.packages("ggplot2")
install.packages("ggrepel")
install.packages("readr")
install.packages("limma")
install.packages("org.Hs.eg.db")
install.packages("tidyverse")
install.packages("enrichR")
install.packages("pathview")
install.packages("org.Mm.eg.db")
install.packages("EBImage")


### Run R Scripts
### Open R scripts in the R/ directory using R Studio. Run the scripts sequentially to execute different parts of the analysis.






````
