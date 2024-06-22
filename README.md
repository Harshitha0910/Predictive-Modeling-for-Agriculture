
# Crop Prediction Based on Soil Measures

Measuring essential soil metrics like nitrogen, phosphorous, potassium levels, and pH value is crucial for assessing soil condition. However, it can be costly and time-consuming, causing farmers to prioritize based on their budget constraints.

Farmers aim to maximize crop yield by considering factors like soil condition, which can be assessed through basic elements such as nitrogen and potassium levels. Each crop has ideal soil conditions for optimal growth and yield.

A farmer requested your assistance as a machine learning expert to select the best crop for his field. The provided dataset, soil_measures.csv, includes:

"N": Nitrogen content ratio in the soil
"P": Phosphorous content ratio in the soil
"K": Potassium content ratio in the soil
"pH": pH value of the soil
"crop": Categorical values representing various crops (target variable)
Each row in the dataset represents soil measurements in a particular field, with the "crop" column indicating the optimal crop choice.

This repository contains a Python script that trains a logistic regression model to predict crop types based on soil measures (N, P, K, and pH levels). The script evaluates each feature's predictive performance and uses the best-performing feature for predictions.

![farmer_in_a_field](https://github.com/Harshitha0910/Predictive-Modeling-for-Agriculture/assets/171827286/37454953-8b20-47ee-bd8f-ea34c31e72ab)

## Description


The script performs the following tasks:

Loads the dataset from a CSV file.

Checks for missing values and prints unique crop types.

Splits the data into training and testing sets.

Trains a logistic regression model for each soil measure feature (N, P, K, ph) individually and evaluates their performance using F1 Score and Balanced Accuracy.

Identifies the best predictive feature based on the highest F1 Score.

Retrains the logistic regression model using the entire dataset for the best feature.

Provides a function to predict the crop type based on user input for soil measures.
## Requirements

Jupyter Notebook

Python 3.x

Pandas

Scikit-learn
