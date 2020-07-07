# Project 2 - Ames Housing Data and Kaggle Challenge


**Introduction**

As a data scientist working for a real estate investment firm, our task is to develop a model to predict the selling price of a given home in Ames, Iowa from 2006 to 2010. Our employer hopes to use this information to help assess whether asking price of a house is higher or lower than the true value of the house. If the home is undervalued, it may be a good investment for the firm. One might wonder what drives the price of a house? The size of the house? Our motivation is to explore and analyze the house dataset to find the key features that influences the sale price and develope  a model to predict in house price in Iowa.



**Dataset**

As described on the Kaggle competition description page, the data for this project was compiled by Dean De Cock for educational purposes, and it includes 79 predictor variables (house attributes) and one target variable (price). As a result of the educational nature of the competition, the data was pre-split into a training set and a test set; the two datasets were given in the forms of csv files. 

The  objective of this project is to  utilize stastical techniques models to predict the housing price for each home in the dataset. There are a clear that many predictors and different datasets, predicting response variables could fall under the following:
- location variables
- age variables
- lot/land variables
- basement variables
- roof variables
- garage variables
- kitchen variables
- room/bathroom variables
- utilities variables
- external features (pools, porches, etc.) variables
**Work flow**
Our steps towards creating a highly accurate model were as follows:

1. Exploratory Data Analysis (EDA) and Data cleaning
   - Missingness imputation
   - Outlier removal
   - Dummification
2. Feature engineering
   - Add new features
   - Scaling
3. Cross-Validation ( Hyperparameter tuning)
4. Modeling

**Conclusions and Recommendations**


For data cleaning and imputation, the most important thing was to identify the categorical variables and numeric variables. For feature engineering, the data normality for both features and target variables is important to prediction accuracy. We transform to log transform whcih is transforming a higly skewed variabl in to a more normalized dataset.

The most valuable feature in this project is the GrLIvArea while Roof Matl and functional sale are least valuable features. In this project we are predicting the price of houses based the data using the linear regression models ridge and lasso. In ridge model, we are applying the alphas value which is between 0.05 to 100. The main tuning parameter for the ridge model is alpha-regularization paramater that measures how flexible our model is. The higher the regularization the less prone our model will be to overfit. The result showed that lasso has a better performance than ridge becuase it shrinks a relatively unimportant coefficient to zero.
Future work may compare Ames, Iowa to other housing markets or develop a model based on housing data from a larger region or at a national scope and data involving local policy changes and economic trends in the housing market. Adding more variables such as school zoning or transportation and commercial information would produce models with more predictive power. Additionally, time-series analysis to predict when is the best time (season) to buy a house.
