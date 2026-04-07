Dataset: Wine Dataset
Source: UCI Machine Learning Repository
Dataset link: https://archive.ics.uci.edu/ml/datasets/wine
Use case: Feature reduction and visualization of high-dimensional data

Columns:
Alcohol
Malic acid
Ash
Alcalinity of ash
Magnesium
Total phenols
Flavanoids
Nonflavanoid phenols
Proanthocyanins
Color intensity
Hue
OD280/OD315 of diluted wines
Proline

Step 1: Data Loading and Understanding
1.1 Load the dataset using pandas
1.2 Display the first 10 rows
1.3 Print dataset shape
1.4 Display column names and data types
1.5 Check for missing values

Step 2: Data Preparation
2.1 Remove duplicate rows (if any)
2.2 Handle missing values
2.3 Separate features from target label (ignore label for unsupervised learning)
2.4 Normalize features using StandardScaler
2.5 Verify scaling using summary statistics

Step 3: Exploratory Data Analysis
3.1 Analyze distributions of numerical features
3.2 Identify highly correlated features
3.3 Visualize feature relationships
3.4 Detect potential outliers

Step 4: Principal Component Analysis (PCA)
4.1 Apply PCA on standardized data
4.2 Compute explained variance ratio
4.3 Determine the number of components required to retain at least 90% variance
4.4 Transform data using selected components
4.5 Interpret principal components

Step 5: Visualization and Analysis
5.1 Visualize data in 2D using first two principal components
5.2 Compare original feature space vs reduced space
5.3 Discuss benefits of dimensionality reduction
5.4 Identify limitations of PCA
