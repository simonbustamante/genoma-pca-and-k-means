# MIT Case Study 1.1: Deciphering the Genome via PCA and K-Means

This Jupyter notebook is a guide to executing a genetic sequencing data analysis using Python libraries such as `requests`, `numpy`, `pandas`, `matplotlib`, `sklearn`, and `termcolor`. The study focuses on the genomic data of *Caulobacter Crescentus*, available for download through a provided link.

## Notebook Setup
The notebook begins by importing necessary libraries and setting up the environment for data analysis. After successful library imports, indicated by a confirmation message, the data acquisition process commences.

## Data Download
The genomic sequencing data for *Caulobacter Crescentus* is retrieved using the `requests` library. The data is formatted into a Python string for subsequent analysis. The script displays both the length and a preview of the sequencing data.

## Feature Generation
The notebook introduces a custom function, `CalcFreq`, inspired by a Matlab function from the case study, to generate features for genome fragments. This function segments the genome into fragments and calculates the frequency of specified subword lengths within each fragment. Feature matrices for different subword lengths (1 to 4) are generated for further analysis.

## PCA (Principal Component Analysis)
Principal Component Analysis (PCA) is applied to reduce the dimensionality of the feature matrices. The notebook demonstrates how to standardize the data and compute the principal components using `sklearn`. It includes visualization functions to plot the PCA results for each subword length.

## K-Means Clustering
The notebook then applies K-Means clustering to the feature matrix with three-letter subwords, focusing on the clustering of the 64 attributes. It demonstrates how to visualize the clustering results both in PCA-reduced space and directly on the genetic sequencing, highlighting different clusters with colors.

## Additional Tasks
The notebook suggests further tasks for exploration, such as determining the optimal number of clusters using methods like the elbow method and visualizing Sum of Squared Errors (SSE) for different cluster counts. It provides sample code for these analyses, encouraging deeper investigation into the genomic data clustering.

In conclusion, this notebook serves as a comprehensive guide for analyzing genetic sequencing data using PCA and K-Means, showcasing the process from data retrieval to advanced clustering analysis.
