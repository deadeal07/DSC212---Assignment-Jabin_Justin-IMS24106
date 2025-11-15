# DSC212---Assignment-Jabin_Justin-IMS24106

# DSC212: Spectral Modularity on the Karate Club Graph

This repository contains the solution for the Research Assignment for DSC212: Graph Theory. The project implements a recursive spectral partitioning algorithm to detect communities in Zachary's Karate Club graph.

The solution is contained entirely within the Jupyter Notebook: `DSC212_ASSIGNMENT_IMS24106.ipynb`

## Project Overview

The goal of this assignment is to implement a community detection algorithm based on **spectral modularity partitioning**. We start with the classic Zachary's Karate Club graph and recursively split it into smaller communities by analyzing the eigenvectors of the modularity matrix ($B$).

## Key Tasks

This notebook successfully completes all the required tasks:
1.  **Implement Recursive Spectral Partitioning:** A function that recursively splits graph communities based on the leading eigenvector of the restricted modularity matrix ($B^{(C)}$).
2.  **Visualize Community Splits:** The graph is plotted after each successful split, showing the new communities in different colors. A fixed layout is used so only the colors change.
3.  **Compute Node Metrics:** At each iteration, four key metrics are computed for all nodes:
    * Degree Centrality
    * Betweenness Centrality
    * Closeness Centrality
    * Clustering Coefficient
4.  **Plot Metric Evolution:** Four line plots are generated to show how these metrics evolve for each node across the iterations. The key nodes (0 and 33) are highlighted.
5.  **Final Discussion:** A written analysis discusses which nodes remain central and how community structure influences the observed metrics.

##  How to Run

1.  Clone this repository.
2.  Open the `.ipynb` notebook file in a compatible environment (like Google Colab, VS Code, or Jupyter Lab).
3.  Run the cells from top to bottom. The notebook is designed to run sequentially without any manual edits.

##  Libraries Used

* `networkx` (for graph operations and metrics)
* `numpy` (for matrix algebra)
* `matplotlib` & `seaborn` (for visualizations)
* `pandas` (for organizing metrics data)
* `scipy` (for efficient eigenvalue computation)
