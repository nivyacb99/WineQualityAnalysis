# WineQualityAnalysis

Project Overview
This project explores the Red Wine Quality dataset using Python, NumPy, and Pandas. It applies fundamentally
Dataset
- File: winequality-red.csv
- Samples: 1,599
- Columns: 12 (11 chemical features and 1 quality target)
- Target Variable: quality
Features include fixed acidity, volatile acidity, citric acid, residual sugar, chlorides, free sulfur dioxide, total sulfur dioxide, density, pH, sulphates, and alcohol.
Objectives
- Load the dataset and check for missing values.
- Replace missing numerical values with the mean of their respective columns.
- Extract alcohol and citric acid as NumPy vectors.
- Select two features (alcohol and density) and calculate their covariance matrix.
- Perform eigen decomposition of the covariance matrix and identify eigenvalues and corresponding eigenvectors.
- Find the most common wine quality score and interpret its distribution.
Analysis and Methods
1. Missing-Value Handling

Checked missing values using Pandas and applied mean imputation using . The dataset has no missing values, so no values were changed.fillna()

2. Vector Extraction

Extracted the alcohol and citric acid columns as NumPy arrays to represent each feature as a vector.

3. Covariance Matrix

Selected alcohol and density as a two-feature matrix and computed the covariance matrix using 'np.cov. Covariance indicates how two features vary together.np.cov(X.T)

4. Eigen Decomposition

Performed eigen decomposition on the covariance matrix using NumPy. Sorted eigenvalues in descending order and reordered the corresponding eigenvectors.

5. Wine Quality Distribution

Used  to count each quality score and identify the most frequent score.value_counts()
Key Findings
- The dataset contains 1,599 samples and 12 columns.
- No missing values were detected in the dataset.
- The most frequent quality score is 5, with 681 samples.
- Quality scores 5 and 6 account for most samples.
- The dataset contains fewer wines at the lowest and highest quality scores.
- Most wines fall within the medium-quality range.
Tools and Libraries
- Python
- Pandas
- NumPy
- Jupyter Notebook
