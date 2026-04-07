Columns:
ORDERNUMBER – unique order identifier
QUANTITYORDERED – number of units sold
PRICEEACH – price per unit
ORDERLINENUMBER – order line number
SALES – total sales value for the order line
ORDERDATE – date when the order was placed
STATUS – order status (Shipped, Cancelled, On Hold, etc.)
QTR_ID – quarter of the year (1–4)
MONTH_ID – month of the year (1–12)
YEAR_ID – year of the order
PRODUCTLINE – product category
MSRP – manufacturer’s suggested retail price
PRODUCTCODE – unique product identifier
CUSTOMERNAME – customer name
PHONE – customer phone number
ADDRESSLINE1 / ADDRESSLINE2 – customer address
CITY – customer city
STATE – customer state
POSTALCODE – postal code
COUNTRY – customer country
TERRITORY – sales territory
CONTACTLASTNAME / CONTACTFIRSTNAME – customer contact person
DEALSIZE – size of the deal (Small, Medium, Large)

Task 1: Data Loading
1.1 Load the dataset using pandas.
1.2 Display the first 10 rows of the dataset.
1.3 Print the shape of the dataset.
1.4 Display column names and data types.
1.5 Check for missing values in each column.

Task 2: Data Cleaning & Preparation
2.1 Check for duplicate ORDERNUMBER and ORDERLINENUMBER combinations.
2.2 Remove duplicate records if any exist.
2.3 Convert ORDERDATE to datetime format.
2.4 Verify that QUANTITYORDERED, PRICEEACH, and SALES are positive.
2.5 Handle missing values in address-related columns (optional).

Task 3: Descriptive Statistics
3.1 Compute mean, median, and standard deviation for:
    QUANTITYORDERED
    PRICEEACH
    SALES
3.2 Find minimum and maximum sales value.
3.3 Group data by COUNTRY and calculate total sales.
3.4 Group data by PRODUCTLINE and compute total quantity sold.

Task 4: Exploratory Data Analysis
4.1 Analyze sales distribution across different years.
4.2 Compare sales performance by deal size.
4.3 Identify top 5 countries by total revenue.
4.4 Analyze average order quantity per product line.

Task 5: Data Visualization
5.1 Plot a histogram of SALES.
5.2 Create a boxplot of PRICEEACH by PRODUCTLINE.
5.3 Plot a time-series chart of monthly total sales.
5.4 Create a bar chart showing total sales by territory.

Task 6: Feature Engineering
6.1 Create a new feature total_revenue_check:
total_revenue_check = QUANTITYORDERED × PRICEEACH
Compare it with SALES.
6.2 Extract order_month and order_year from ORDERDATE.
6.3 Create a binary feature large_deal_flag:
1 if DEALSIZE = "Large"
0 otherwise
6.4 Encode categorical variables (PRODUCTLINE, COUNTRY, DEALSIZE).

Task 7: Correlation Analysis
7.1 Compute correlation matrix for numerical features.
7.2 Visualize correlations using a heatmap.
7.3 Identify features most correlated with SALES.

Task 8: Train–Test Split
8.1 Define the target variable as SALES.
8.2 Select appropriate input features.
8.3 Split the dataset into training and testing sets (80/20).

Task 9: Regression Modeling
9.1 Train a Linear Regression model to predict SALES.
9.2 Train an additional model (Ridge / Random Forest Regressor).
9.3 Evaluate models using:
Mean Absolute Error (MAE)
Mean Squared Error (MSE)
R² Score
