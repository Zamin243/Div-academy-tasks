Dataset: Online Retail Dataset Dataset link: https://archive.ics.uci.edu/ml/datasets/online+retail Use case: Customer purchasing behavior analysis and segmentation

Columns: InvoiceNoStockCode Description Quantity InvoiceDate UnitPrice CustomerID Country

Step 1: Data Loading and Understanding 1.1 Load the dataset using pandas 1.2 Display the first 10 rows 1.3 Print dataset shape 1.4 Display column names and data types 1.5 Check for missing values

Step 2: Data Cleaning and Preparation 2.1 Check for duplicate rows 2.2 Remove cancelled transactions (negative Quantity) 2.3 Handle missing CustomerID values 2.4 Aggregate transactional data at customer level 2.5 Normalize numerical features using StandardScaler

Step 3: Exploratory Data Analysis 3.1 Analyze distribution of purchase quantities and prices 3.2 Identify skewed features 3.3 Visualize relationships between aggregated customer features 3.4 Detect potential outliers in spending behavior

Step4: K-Means Clustering 4.1 Apply K-Means clustering on customer-level features 4.2 Determine optimal number of clusters using: Elbow Method Silhouette Score 4.3 Train K-Means with optimal K 4.4 Assign cluster labels 4.5 Interpret cluster centroids

Step 5: Hierarchical Clustering 5.1 Perform Agglomerative Clustering 5.2 Experiment with linkage methods (ward, average, complete) 5.3 Plot dendrogram 5.4 Determine optimal number of clusters 5.5 Compare results with K-Means
