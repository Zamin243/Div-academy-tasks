Dataset: Breast Cancer Wisconsin (Diagnostic) Dataset
Source: UCI Machine Learning Repository / scikit-learn
Dataset link: https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_breast_cancer.html
Use case: Feature reduction and structure analysis of medical tabular data
Dataset Description: The dataset contains numeric measurements of cell nuclei from breast cancer biopsies.
It includes 30 numerical features, making it small, tabular, and ideal for PCA.

Columns (examples):
Radius
Texture
 Perimeter
Area
Smoothness
Compactness
Concavity
Symmetry
Fractal Dimension
(and similar measurements)

Note: Class labels exist but should be ignored for PCA.

Step 1: Data Loading and Understanding
1.1 Load the dataset using pandas / scikit-learn
1.2 Display the first 10 rows
1.3 Print dataset shape
1.4 Display feature names and data types
1.5 Check for missing values

Step 2: Data Cleaning and Preparation
2.1 Verify that all features are numerical
2.2 Check for duplicate rows
2.3 Handle missing values (if any)
2.4 Standardize features using StandardScaler
2.5 Verify scaling using summary statistics

Step 3: Exploratory Data Analysis
3.1 Analyze summary statistics of features
3.2 Identify features with high variance
3.3 Examine correlations between features
3.4 Discuss redundancy in tabular data

Step 4: Principal Component Analysis (PCA)
4.1 Apply PCA on standardized data
4.2 Compute explained variance ratio for each principal component
4.3 Plot cumulative explained variance
4.4 Determine the minimum number of components required to retain at least 90% variance
4.5 Transform the dataset using selected principal components

Step 5: Visualization and Analysis
5.1 Visualize data using the first two principal components
5.2 Analyze structure and separation in reduced space
5.3 Compare dimensionality before and after PCA
5.4 Discuss information loss due to dimensionality reduction
