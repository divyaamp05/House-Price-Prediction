# House-Price-Prediction

This repository contains Project on predicting house prices using advanced data analysis and machine learning techniques. The primary goal is to build a model that can accurately estimate the price of a house based on various features such as location, size, number of bedrooms, and more.

## Dataset

The dataset used in this project includes various features such as:
- Location
- Area
- Interior Spaces
- LandSlope
- Age of the house
- Other relevant features

## Code

The main code for the House Price Prediction is implemented in House Price Prediction.ipynb. 
This Jupyter Notebook contains the following sections:

## Exploratory Data Analysis

Exploratory Data Analysis (EDA) is a crucial step in understanding the data and preparing it for modeling. The EDA for this project is divided into several steps:

### Missing Values Analysis

The first step in EDA is to analyze the missing values in the dataset. Understanding which features have missing values and how many of them are missing helps in deciding the imputation strategy.

1. *Identify Missing Values*: Check for missing values in the dataset.
2. *Visualize Missing Values*: Draw a graph to visualize the missing values and their impact on the output variable (house price).

### Numerical Variables

Numerical variables are analyzed by dividing them into temporal variables, discrete variables, and continuous variables.

#### a.Temporal Variables

Temporal variables are features that represent time or date-related information.

1. *Identify Temporal Variables*: Determine which features are temporal.
2. *Visualize Temporal Variables*: Plot graphs between temporal variables and the output variable to understand their relationship.

#### b.Discrete Variables
Discrete variables are numerical variables that take on a limited number of distinct values.

1. *Identify Discrete Variables*: Determine which features are discrete.
2. *Visualize Discrete Variables*: Plot graphs between discrete variables and the output variable to understand their relationship.

#### c.Continuous Variables
Continuous variables are numerical variables that can take on any value within a range. Proper handling and transformation of these variables are crucial for building an effective predictive model. Below are the steps taken to manage continuous variables in this project:

1. *Identify Continuous Variables*: Determine which features in the dataset are continuous. These variables are typically numerical and can have a wide range of values.

2. *Visualize Continuous Variables*: Plot graphs between continuous variables and the output variable to understand their relationship. This helps in observing correlations and distributions, and includes visualizations like scatter plots and histograms.

3. *Lognormal Transformation*: Apply lognormal transformation to continuous variables to normalize their distribution. This transformation can help in handling skewed data and making the features more normally distributed.

4. *Outlier Detection*: Use boxplots to detect outliers in the continuous variables. Outliers can significantly affect the performance of the model, so identifying and handling them is crucial.

### Categorical Variables
Categorical variables are non-numerical features that represent categories or groups.

1. *Identify Categorical Variables*: Determine which features are categorical.
2. *Visualize Categorical Variables*: Plot graphs between categorical variables and the output variable to understand their relationship.

## Feature Engineering
Feature engineering involves transforming raw data into meaningful features that improve the performance of machine learning models.

### 1.*Handling Categorical Variables*
Categorical variables are first handled for missing values by converting them into non-missing values. Then, label encoding is performed to convert categorical variables into numerical form.

### 2.*Handling Numerical Variables*
Numerical variables are handled for missing values by filling them with zero.

### 3.*Feature Scaling*
Feature scaling is performed to normalize the range of independent variables or features of the data. Min-Max scaling is applied using MinMaxScaler() to scale the features and transform them into a data frame.

### 4.*Feature Selection*
Feature selection is performed using LASSO regression model to select the most important features. Out of 81 features, only 74 are selected based on the model.

## Model Training
We trained a linear regression model on the processed dataset. The steps involved:
1. Splitting the data into training and testing sets.
2. Training the model on the training set.
3. Evaluating the model on the testing set.

## Performance Metrics
We used the following performance metrics to evaluate the model:
- **R-squared (R²)**: Measures the proportion of variance in the dependent variable that is predictable from the independent variables.
- **Adjusted R-squared**: Adjusts the R-squared value based on the number of predictors in the model.

## Results
The model achieved the following performance metrics:
- **R-squared**: 0.73
- **Adjusted R-squared**: 0.68

These metrics indicate that the model has strong predictive capabilities.

## Dependencies

- Python 3
- Jupyter Notebook
- scikit-learn
- Pandas
- NumPy
- Matplotlib
- Seaborn

## How to Run the Project
1. Clone the repository:
   ```
   git clone https://github.com/yourusername/house-price-prediction.git
   ```
2. Navigate to the project directory:
   ```
   cd house-price-prediction
   ```
3. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```
4. Run the Jupyter notebooks or Python scripts in the `notebooks/` or `scripts/` directory to see the analysis and model training steps.

## Conclusion
This project demonstrates the process of building a house price prediction model using data preprocessing, feature engineering, and machine learning techniques. The model provides accurate predictions and can be further improved with additional data and advanced modeling techniques.

## Contributions
Contributions to improve the project are welcome! Feel free to submit issues for bugs or feature requests, and pull requests are encouraged for implementing new features or addressing existing issues.
