# Penguin Clustering Project

## Overview

This project uses KMeans clustering to classify penguins based on their physical features, such as bill length, bill depth, flipper length, and body mass. The project includes the implementation of the **Elbow Method** to determine the optimal number of clusters and visualizes the results.

## Dataset

The dataset used in this project is the **Penguins dataset** from the **Seaborn** library, which contains information about different penguin species and their physical characteristics.

### Features:

- `bill_length_mm`: Length of the bill (in mm)
- `bill_depth_mm`: Depth of the bill (in mm)
- `flipper_length_mm`: Length of the flipper (in mm)
- `body_mass_g`: Mass of the penguin (in grams)
- `species`: Species of the penguin (categorical feature)

## Clustering Approach

### Steps:

1. **Data Preprocessing**: The dataset is cleaned by removing any rows with missing values.
2. **Feature Selection**: The relevant features are selected for clustering: `bill_length_mm`, `bill_depth_mm`, `flipper_length_mm`, and `body_mass_g`.
3. **Standardization**: The features are standardized using **StandardScaler** to ensure that all features contribute equally to the clustering process.
4. **Elbow Method**: The **Elbow Method** is applied to determine the optimal number of clusters (`k`). This method involves plotting the **Within-Cluster Sum of Squares (WCSS)** and identifying the "elbow point" where the WCSS begins to decrease more slowly.
5. **KMeans Clustering**: **KMeans** is used for clustering the penguins into groups based on their physical features.
6. **Visualization**: The resulting clusters are visualized using a 2D scatter plot. The clusters are color-coded for easy interpretation.

## Requirements

- Python 3.x
- Libraries:
  - Seaborn
  - Pandas
  - Matplotlib
  - Scikit-learn
  - IPython

## How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/Rahul0015/penguin_clusteringKM.git
   ```
