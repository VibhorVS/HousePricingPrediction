# Bengaluru House Prices Prediction

This repository contains code for predicting house prices in Bengaluru using machine learning. The dataset used for this project is "bengaluru_house_prices.csv."

## Prerequisites

Before running the code, make sure you have the following libraries installed:
- pandas
- numpy
- matplotlib
- scikit-learn

## Code Overview

The code in this repository is structured as follows:

### 1. Data Preprocessing
   - The dataset is loaded using the pandas library, and an initial exploration is conducted to gain insights into the data.
   - Data cleaning and preprocessing steps are performed to address missing values and outliers, ensuring the data is in a suitable format for machine learning.

### 2. Data Visualization
   - The code utilizes the matplotlib library to create various visualizations that help in understanding the dataset better. Visualizations include:
     - Scatter plots: These are used to explore relationships between variables, such as the square footage and price per square foot.
     - Histograms: These show the distribution of house prices and other relevant features.
     
### 3. Feature Engineering
   - Feature engineering is a crucial step in preparing the data for modeling. In this section, we perform the following tasks:
     - Create dummy variables for location: Location is an important predictor, so we convert categorical location data into numerical form for model training.
     - Remove unnecessary columns: Columns like "size," "price_per_sqft," and others are dropped to focus on the essential features.

### 4. Model Building
   - Machine learning models are trained to predict house prices. Specifically, we employ a linear regression model for this task. The linear regression model learns patterns in the data to make predictions based on input features.

### 5. Model Evaluation
   - To assess the performance of our model, we use cross-validation techniques. This ensures that the model's accuracy is robust and not overfitting or underfitting the data.
   - Grid search is applied to fine-tune hyperparameters, optimizing the model's performance.

### 6. Prediction Function
   - We define a function called `predict_price` that allows users to make price predictions based on input parameters:
     - Location: The area where the property is located.
     - Square footage: The total square footage of the property.
     - Number of bathrooms: The count of bathrooms in the property.
     - Bedrooms (BHK): The number of bedrooms in the property.

The code is structured to provide a comprehensive analysis of house prices in Bengaluru, from data preprocessing to model training and prediction. The accuracy of the predictions is dependent on the quality of the data and the chosen machine learning model.

