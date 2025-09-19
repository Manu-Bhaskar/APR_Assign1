# PCA (Principal Component Analysis) Implementation

This project demonstrates the implementation of Principal Component Analysis (PCA) from scratch on a dataset, including data preprocessing, covariance matrix calculation, eigen decomposition, explained variance analysis, and data transformation.

## Contents

- Dependencies
- Dataset Reading
- Data Standardization
- Covariance Matrix Calculation
- Eigenvalues and Eigenvectors Computation
- Explained Variance Analysis
- Principal Components Calculation
- Summary and Interpretation

## Dependencies

The implementation uses the following Python libraries:

- `numpy` for numerical operations
- `pandas` for data handling

## Dataset

The dataset used consists of multiple features (x1 to x15) and a target variable `y`. It is loaded from a CSV file and displayed partially to show the structure.

## Steps

### 1. Reading the Dataset

The dataset is read into a Pandas DataFrame and the first few rows are displayed for initial inspection.

### 2. Data Standardization

The feature columns are standardized by subtracting the mean and dividing by the standard deviation to ensure zero mean and unit variance, which is essential for PCA.

### 3. Covariance Matrix Calculation

The covariance matrix is computed from the standardized data to capture the relationships between features.

### 4. Eigenvalues and Eigenvectors

The eigenvalues and eigenvectors of the covariance matrix are calculated using numerical linear algebra routines. The eigenvalues represent the amount of variance explained by each principal component.

### 5. Explained Variance

The explained variance ratio for each principal component is calculated and cumulative explained variance is computed. This helps determine how many principal components capture most of the data variance. In this project, 10 components are chosen as they explain about 90% of the variance.

### 6. Principal Components Calculation

The standardized data is projected onto the top principal components, yielding transformed data in the reduced-dimension space.

### 7. Summary

PCA effectively summarizes the dataset by removing redundancy and converting correlated features to orthogonal components. Components with high eigenvalues capture the most variation in data, facilitating dimensionality reduction and visualization.