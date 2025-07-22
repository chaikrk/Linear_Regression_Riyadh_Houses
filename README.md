# Riyadh Real Estate Apartment Price Prediction

This project aims to predict apartment sellinga prices in Riyadh, Saudi Arabia, using a linear regression model.

## Project Overview

The project utilizes a dataset containing information about apartments for sale in Riyadh, including features like area, number of bedrooms and bathrooms, location (neighborhood, latitude, longitude), and property age. The goal is to build a model that can accurately estimate the selling price of an apartment based on these features.

## Data

The dataset used in this project is sourced from Kaggle:
- `riyadh_apartments_data.csv`: Contains details about the apartments.
- `riyadh_geocoding.csv`: Provides geographical coordinates for neighborhoods.

The data undergoes preprocessing steps including:
- Merging the two datasets.
- Handling missing values (if any).
- Encoding categorical features.
- Dropping irrelevant columns.
- Log-transforming the target variable (`Selling Price (SAR)`) to address skewness.

## Methodology

A linear regression model is trained on the preprocessed data to predict the log-transformed selling price. The model's performance is evaluated using the following metrics:
- Root Mean Squared Error (RMSE)
- R-squared (R²)

## Results

The linear regression model achieved an R-squared score of 0.95 on the test set, indicating that approximately 95% of the variance in the log-transformed selling price can be explained by the model. The RMSE was 0.19 SAR, representing the typical difference between the predicted and actual log-transformed prices.

