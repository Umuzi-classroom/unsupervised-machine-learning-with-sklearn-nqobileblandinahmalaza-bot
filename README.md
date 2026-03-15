[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/wvwe4VzF)
# Unsupervised Learning Assessment

**Dataset**: [Wholesale Customers Dataset (UCI)](https://archive.ics.uci.edu/dataset/292/wholesale+customers)

**Goal**: Use unsupervised learning techniques to identify meaningful customer segments and reflect on the structure and variance within the data.

In this assessment, you will:

- Preprocess and explore the data  

- Apply dimensionality reduction using **Principal Component Analysis (PCA)  
    **
- Use **KMeans clustering** to identify customer segments  

- Evaluate clustering performance  

- Visualize and interpret your results  

Your approach should reflect strong data science thinking: balancing theory, execution, and business-like interpretation.

## Task Breakdown

### Data Preparation

- Load the dataset and explore its structure.  

- Handle any necessary preprocessing:  
  - Decide how to treat the Channel and Region columns.  

  - Ensure the data is appropriately scaled before applying PCA or clustering.

Deliverable: Cleaned and scaled dataset ready for analysis.

### Dimensionality Reduction (PCA)

- Apply PCA to the scaled dataset.  

- Determine how many principal components are needed to capture most of the variance.  

- Create a screen plot to visualize the explained and cumulative variance.

Deliverable: Summary of variance explained by components and your rationale for how many components to retain.

### Clustering (KMeans)

- Apply the KMeans algorithm to segment the data.  

- Test different values of _k_ (number of clusters) and evaluate performance using:  
  - **Inertia (SSE)**
  - **Silhouette Score**
- Determine the most appropriate number of clusters and justify your choice.

Deliverable: Plots for inertia and silhouette score with an explanation of how you chose _k_.

### Compare Clustering Performance: Raw vs PCA-Reduced Data

After identifying your optimal number of clusters, compare how well the clustering performs when applied to:

- The **original scaled dataset**
- The **PCA-reduced dataset** (using the number of components you selected earlier)  

You should:

- Fit separate KMeans models on each dataset  
- Evaluate both models using the **silhouette score**
- Reflect on the tradeoffs: does dimensionality reduction improve or hurt cluster structure?  

Deliverable: A short comparison of silhouette scores with and without PCA, and your interpretation of the result

### Cluster Visualization

- Use PCA (first 2 components) to visualize the clusters in 2D space.  

- Plot the customer data points, colored by cluster label.  

Deliverable: Visual chart of clusters in PCA space.

### Principal Component Interpretation

- Examine the components to understand which features contribute most to PC1 and PC2.  

- Reflect on what those components represent and how they help interpret the clusters visually.  

Deliverable: Short explanation of what PC1 and PC2 represent based on feature contributions.

### Cluster Insights

- Analyze and describe the characteristics of each cluster.  

- Which features distinguish them? What behaviors or strategies might each group represent?  

- Reflect on what business decisions might be informed by these clusters.  

Deliverable: A summary of your insights on each customer segment(within the same notebook!).
