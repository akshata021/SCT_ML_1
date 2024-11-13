Project: Predicting House Prices with Linear Regression
In this project, we aim to build a linear regression model that predicts house prices based on key property features such as square footage, the number of bedrooms, and the number of bathrooms. This type of predictive modeling can be useful for real estate companies, property assessors, and potential homebuyers interested in estimating a home’s value given certain features.

Project Overview
Goal: Predict the sale price of a house.
Dataset: Contains details about houses, including:
GrLivArea: Square footage of the house.
BedroomAbvGr: Number of bedrooms above ground.
FullBath and HalfBath: Number of full and half bathrooms.
SalePrice: The actual sale price of the house (our target variable).
Approach: Using a linear regression model, which assumes a linear relationship between the features and the target (house price).

Project Steps :
Data Loading and Preparation -
Load the dataset from a CSV file into a pandas DataFrame and select only the relevant features. For simplicity, in this project, we are not performing additional cleaning steps such as handling missing values or feature engineering.

Feature Selection -
We are focusing on three primary predictors:
GrLivArea: Square footage, which is generally one of the strongest indicators of price.
BedroomAbvGr: Number of bedrooms, which affects how desirable a home is to families.
FullBath and HalfBath: Combined to create a total bathroom count, a standard feature in real estate pricing.

Train-Test Split -
Split the data into training and testing sets to evaluate how well the model generalizes to unseen data. Here, we use 80% of the data for training and 20% for testing.

Model Training -
Train the model using the training data. The model learns the best values for the intercept and coefficients to minimize the error between predicted and actual house prices.

Model Prediction -
Use the trained model to predict house prices on the test set.

Model Evaluation -
Assess the model’s accuracy and performance using:
Mean Squared Error (MSE): Measures the average squared difference between predicted and actual values.
Mean Absolute Error (MAE): Measures the average absolute difference between predicted and actual values.
R-squared (R²): Indicates the proportion of the variance in the target variable explained by the features.

Data Visualization -
Actual vs. Predicted Prices: A scatter plot showing the relationship between actual sale prices and predicted prices, with a reference line where predicted values equal actual values.
Residuals Distribution: Plotting residuals (errors) to analyze how predictions deviate from actual prices, ideally centered around zero.
