# textual-data-visualization-and-clustering

# Textual Data Structure Discovery via Unsupervised Learning

This project explores how unsupervised learning methods can reveal patterns in high-dimensional textual data. It applies a variety of dimensionality reduction and clustering techniques to chapter-level word frequency data from famous authors.

---

## Methods Used

- **Dimensionality Reduction:** PCA, UMAP, MDS, Spectral Embedding, NMF
- **Clustering Algorithms:** KMeans, Spectral Clustering, GMM, Agglomerative Clustering
- **Pattern Mining:** Mutual Information, Biclustering
- **Validation:** Silhouette Analysis, Consensus Matrices, Stability Scores

---

## Key Results

- **UMAP** produced the clearest and most compact author clusters among dimensionality reduction methods.
- **Spectral Clustering** achieved the best classification (Accuracy = 99.5%, ARI = 0.985).
- **Mutual Information** revealed that words like *“was”, “the”, “her”* were highly discriminative for author identity.
- **Stability & Silhouette** validation both selected K=4 as optimal number of clusters.

---

## Visualizations

### 1. Author Clustering with PCA, UMAP, MDS, Spectral Embedding
![Embedding Comparison](images/author_embedding_grid.png)

### 2. Word Embeddings with PCA, UMAP, NMF
![Word Layout](images/word_embedding_grid.png)

### 3. Biclustering Heatmap
![Heatmap](images/biclustering_heatmap.png)

### 4. Cluster Validation
- Silhouette score peak at K=4
- Consensus matrix confirms clustering stability

---

## Dependencies

Install required packages with:

```bash
pip install -r requirements.txt
