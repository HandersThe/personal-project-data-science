# Penguin Clustering Analysis

This project applies unsupervised learning techniques to perform cluster analysis on the "penguins.csv" dataset.

## Project Objective

The main goal of this project is to identify and analyze clusters within the penguin dataset using unsupervised learning methods.

## Key Steps

1. Import, investigate, and pre-process the "penguins.csv" dataset.
2. Perform cluster analysis using a reasonable number of clusters.
3. Collect and analyze the average values for each cluster.

## Output

The primary output of this analysis is a DataFrame named `stat_penguins` with the following characteristics:
- One row per identified cluster
- Columns representing the mean of the original numeric variables from "penguins.csv" for each cluster
- Non-numeric columns from the original dataset are excluded

## Getting Started

### Prerequisites

- Python enviroment
- pandas
- matplotlib
- scikit-learn

Or just use Google colab for ease of use.

## Methodology

1. **Data Preprocessing**: 
   - Handle missing values (if necessary)
   - Encode categorical variables
   - Standardize numeric features

2. **Clustering Algorithm**: 
   - The project uses k-means clustering
   - The number of clusters is determined by elbow method

3. **Analysis**:
   - Calculate mean values of numeric features for each cluster

## Results

After running the analysis, you'll find:
- The `stat_penguins` DataFrame containing mean values for each cluster

## Acknowledgments

- The Palmer Penguins dataset by Allison Horst, Alison Hill, and Kristen Gorman