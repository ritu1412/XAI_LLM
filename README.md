# Embedding Visualization and XAI Prompting

This repository contains resources for visualizing embeddings and exploring explainable AI (XAI) prompting methods. The project leverages various dimensionality reduction techniques to visualize embedding spaces and applies XAI techniques to analyze the key components of prompts. 

## Folder Structure

├── data                        # Folder for data file in tsv
├── embeddings                  # Contains embedding visualizations
│   ├── pca.tsv                 # Embeddings reduced with PCA
│   ├── tsne.tsv                # Embeddings reduced with t-SNE
│   └── umap.tsv                # Embeddings reduced with UMAP
├── requirements.txt            # Required libraries
├── notebooks                   # Jupyter notebooks for analysis
│   ├── embedding_visualisation.ipynb  # Notebook for embedding visualization
│   └── xai_prompting.ipynb     # Notebook for XAI prompting analysis
└── README.md                   # Project documentation

## Project Overview

This project is split into two main areas:
1. **Embedding Visualization**: Visualize the embedding space using different dimensionality reduction techniques like PCA, t-SNE, and UMAP. 
2. **XAI Prompting**: Use explainable AI methods to analyze and interpret various prompt components, helping us understand symbols, patterns, and text effects in the prompt space.

### Embedding Visualizations

- **PCA (`pca.tsv`)**: Principal Component Analysis (PCA) for reducing high-dimensional embeddings into two dimensions.
- **t-SNE (`tsne.tsv`)**: t-Distributed Stochastic Neighbor Embedding (t-SNE) for visualizing embeddings in 2D, focusing on preserving local structure.
- **UMAP (`umap.tsv`)**: Uniform Manifold Approximation and Projection (UMAP) for dimensionality reduction, which aims to maintain both local and global structure.

The visualizations are saved as `.tsv` files in the `embeddings` folder and can be viewed through `embedding_visualisation.ipynb`.

### XAI Prompting

In the `xai_prompting.ipynb` notebook, XAI technique perturbations is applied to analyze key components in prompts, such as symbols, patterns, and text. This helps in understanding the model's interpretation of different prompt variations.

## Setup Instructions

1. **Clone the Repository**:
   ```bash
   git clone <repository_url>
   cd <repository_name>
   ```

2. **Install Dependencies**:
   Additional dependencies are required, you can install them using:
   pip install -r requirements.txt

4. **Running Jupyter Notebooks**:
   Start Jupyter Notebook to explore and run the provided notebooks:
   Open `embedding_visualisation.ipynb` or `xai_prompting.ipynb` from the `notebooks` folder.

## Notebooks

- **embedding_visualisation.ipynb**: This notebook loads pre-computed embeddings (PCA, t-SNE, UMAP) and visualizes them. You can also compare the effectiveness of these dimensionality reduction techniques.
  
- **xai_prompting.ipynb**: This notebook explores prompt analysis with XAI methods, focusing on the impact of different prompt elements (e.g., symbols, patterns, text) on model responses.


## Embedding Files

- The `embeddings` folder contains `.tsv` files for each dimensionality reduction technique:
  - `pca.tsv`: PCA-reduced embeddings
  - `tsne.tsv`: t-SNE-reduced embeddings
  - `umap.tsv`: UMAP-reduced embeddings

These files are loaded within `embedding_visualisation.ipynb` for comparison and visualization.

# Reference
Used GPT4o for making the markdown Table
Other references in colab notebook