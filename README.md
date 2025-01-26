
Weather Forecasting Using Data Science

- Deliverables:
  1. Jupyter Notebook under the Weather folder (data.ipynb)
  2. Presentation file Titled: Data Science Assessment_ Weather Trend Forecasting.pdf
- Project Overview:

Technologies Used
Python: For data analysis, visualization, and modeling.
Pandas: For data manipulation and preprocessing.
Matplotlib/Seaborn: For data visualization and exploratory analysis.
XGBoost: For building an advanced machine learning model.

Data:
I used weather data containing features such as temperature, precipitation, wind direction, and other meteorological attributes. The dataset included both numerical and categorical variables.

I. Data Preprocessing:
Handled missing values appropriately.
Categorical variables were encoded using Label Encoding to prepare them for machine learning model.
Split the data into training and testing sets for performance evaluation (80%, 20%).

II. EDA:
EDA played a crucial role in understanding the structure and relationships within the dataset before building models. Below are the key steps I took during the EDA process:

1. Correlation Analysis: 
I calculated the correlations between numerical features to identify relationships between variables such as temperature, humidity, and precipitation.
Created a heatmap using Seaborn to visually represent these correlations.
Strong positive correlations were observed between temperature and related metrics, indicating dependencies that were leveraged in the machine learning models.
Weak correlations between some features hinted at potential noise or irrelevant variables.
2. Data Visualization:
Used histograms and box plots to understand the distributions of temperature, precipitation, and other weather metrics.
Plotted time series line graphs to observe seasonal and periodic trends in the data.
Generated scatter plots to explore relationships between variables and detect any non-linear patterns.
3. Outlier Detection:
Identified and analyzed outliers using box plots and scatter plots.
Addressed significant outliers to improve model performance while retaining meaningful extreme values that could impact weather forecasting.

III. Model and Results:

I implemented an XGBoost Regressor to predict temperature and precipitation.
Used hyperparameters such as max_depth=5, n_estimators=100, and objective='reg:squarederror'.

Metrics:

Testing Data:

MSE: 0.03898, 
RMSE: 0.1974, 
MAE: 0.0600

Training Data:

MSE: 0.00477, 
RMSE: 0.0690, 
MAE: 0.0425

The XGBoost model performed well, highlighting its strength in capturing patterns in both numerical and categorical data.

IV. Key Insights:
Preprocessing categorical variables is crucial for the performance of machine learning models like XGBoost.
XGBoost was effective at achieving low error rates for both training and testing datasets.
