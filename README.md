Columns:

Gender
Customer Type
Age
Type of Travel
Class
Flight Distance
Inflight wifi service
Seat comfort
Food and drink
Online boarding
Departure Delay in Minutes
Arrival Delay in Minutes
Satisfaction -> target variable
(satisfied / neutral or dissatisfied)


Task 1: Data Loading
1.1 Load the dataset from CSV.
1.2 Display the first 10 rows.
1.3 Print dataset shape.
1.4 Display column names and data types.
1.5 Check missing values for each column.

Task 2: Data Cleaning
2.1 Remove irrelevant columns (e.g., unnamed index columns).
2.2 Handle missing values in delay columns.
2.3 Check for duplicate records and remove if any.
2.4 Ensure rating features are within valid ranges (0–5).
2.5 Convert target variable Satisfaction into binary format.

Task 3: Exploratory Data Analysis
3.1 Compute descriptive statistics for numerical features.
3.2 Analyze satisfaction distribution (class balance).
3.3 Compare satisfaction by:
    Travel type
    Flight class
3.4 Analyze average delays for satisfied vs dissatisfied passengers.

Task 4: Data Visualization
4.1 Bar chart of satisfaction classes.
4.2 Boxplot of flight distance by satisfaction.
4.3 Histogram of passenger age.
4.4 Bar chart of average service ratings (wifi, seat comfort, food).

Task 5: Feature Engineering
5.1 Create a new feature total_delay:
total_delay = Departure Delay + Arrival Delay
5.2 Create binary feature long_flight:
    1 if Flight Distance > median
    0 otherwise
5.3 Encode categorical variables using One-Hot Encoding.
5.4 Scale numerical features where necessary.

Task 6: Correlation & Feature Importance
6.1 Compute correlation matrix for numerical features.
6.2 Visualize correlations using heatmap.
6.3 Identify top features affecting passenger satisfaction.

Task 7: Train–Test Split
7.1 Define target variable as Satisfaction.
7.2 Select appropriate input features.
7.3 Split dataset into training and testing sets (80/20).

Task 8: Classification Modeling
8.1 Train Logistic Regression model.
8.2 Train Random Forest Classifier.
8.3 (Optional) Train XGBoost / Gradient Boosting.
8.4 Compare models using:
    Accuracy
    Precision
    Recall
    F1-score
