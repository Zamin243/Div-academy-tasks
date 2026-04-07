year – year of measurement
month – month of measurement
day – day of month
hour – hour of measurement
station – air quality monitoring station name
PM2.5 – fine particulate matter (µg/m³)
PM10 – inhalable particulate matter (µg/m³)
SO2 – sulfur dioxide concentration
NO2 – nitrogen dioxide concentration
CO – carbon monoxide concentration
O3 – ozone concentration
TEMP – temperature (°C)
PRES – atmospheric pressure (hPa)
DEWP – dew point temperature
RAIN – precipitation (mm)
WSPM – wind speed (m/s)
wd – wind direction

Task 1: Data Loading
1.1 Load the dataset using pandas.
1.2 Display the first 10 rows of the dataset.
1.3 Print the shape of the dataset.
1.4 Display column names and data types.
1.5 Check for missing values in each column.

Task 2: Data Cleaning & Preparation
2.1 Combine year, month, day, and hour into a single datetime column.
2.2 Sort the data chronologically.
2.3 Handle missing values in pollutant and meteorological columns.
2.4 Remove or flag extreme outliers in pollution measurements (optional).
2.5 Ensure all numerical columns have appropriate data types.

Task 3: Exploratory Data Analysis (EDA)
3.1 Compute descriptive statistics for air pollutants.
3.2 Analyze seasonal trends in PM2.5 concentration.
3.3 Compare average pollution levels across stations.
3.4 Analyze relationship between wind speed and PM2.5 levels.

Task 4: Data Visualization
4.1 Plot time-series of PM2.5 for one selected station.
4.2 Create boxplots of PM2.5 grouped by month.
4.3 Plot histogram of PM2.5 concentration.
4.4 Visualize average pollutant levels by station using bar charts.

Task 5: Feature Engineering
5.1 Create a feature datetime from time components.
5.2 Create season feature based on month:
    Winter, Spring, Summer, Autumn
5.3 Create a new feature pollution_load:
    pollution_load = PM2.5 + PM10 + NO2 + SO2 + O3
5.4 Encode wind direction (wd) using appropriate encoding.

Task 6: Correlation Analysis
6.1 Compute correlation matrix for numerical features.
6.2 Visualize correlation matrix using a heatmap.
6.3 Identify meteorological variables most correlated with PM2.5.

Task 7: Train–Test Split
7.1 Define the target variable as PM2.5.
7.2 Select relevant meteorological and temporal features.
7.3 Split data into training and testing sets using a time-based split.

Task 8: Regression Modeling
8.1 Train a Linear Regression model to predict PM2.5.
8.2 Train an additional model (Random Forest Regressor or Gradient Boosting).
8.3 Evaluate models using:
    Mean Absolute Error (MAE)
    Mean Squared Error (MSE)
    R² Score
