# NN and KNN for price prediction.
This project implements and compares Neural Networks (NN) and K-Nearest Neighbors (KNN) to predict vehicle prices based on various attributes such as mileage, body style, number of owners, horsepower, and more. The dataset used for this project comes from Auto Scout Car Price on Kaggle.

Motivation
As an avid car enthusiast, I was particularly interested in leveraging machine learning to analyze car pricing trends. While I initially aimed to work with racing analytics, I pivoted to car price prediction, as it is a widely applicable machine learning problem with potential use cases in pricing recommendations, dealership analysis, and market trend predictions.

Dataset
Source: Kaggle - Auto Scout Car Price Dataset
Size: 15,915 car listings
Features: 22 (including mileage, age, number of gears, trim options, interior features, etc.)
Target Variable: Vehicle Price
The dataset provides a rich set of features, making it well-suited for exploring how different car attributes influence pricing.


Here's a comprehensive README for your GitHub repository based on your project report.

Predicting Auto Prices Using Machine Learning Models: NN and KNN
Overview
This project implements and compares Neural Networks (NN) and K-Nearest Neighbors (KNN) to predict vehicle prices based on various attributes such as mileage, body style, number of owners, horsepower, and more. The dataset used for this project comes from Auto Scout Car Price on Kaggle.

Motivation
As an avid car enthusiast, I was particularly interested in leveraging machine learning to analyze car pricing trends. While I initially aimed to work with racing analytics, I pivoted to car price prediction, as it is a widely applicable machine learning problem with potential use cases in pricing recommendations, dealership analysis, and market trend predictions.

Dataset
Source: Kaggle - Auto Scout Car Price Dataset
Size: 15,915 car listings
Features: 22 (including mileage, age, number of gears, trim options, interior features, etc.)
Target Variable: Vehicle Price
The dataset provides a rich set of features, making it well-suited for exploring how different car attributes influence pricing.

Methods and Models
1. Neural Network (NN)
Implemented using PyTorch
Architecture:
Input layer: Corresponding to the number of features
Two hidden layers with ReLU activation
Output layer: Single neuron for regression
Optimization & Loss Function:
Optimizer: Adam
Loss function: Mean Squared Error (MSE)
Training: 200 epochs with fine-tuned hyperparameters
Scaling: Standard normalization applied to numerical features
2. K-Nearest Neighbors (KNN)
Implemented using scikit-learn
Hyperparameter Tuning: Used GridSearchCV to find the optimal value of k
Distance metric: Euclidean
Scaling: Standard normalization to prevent distance distortion

Preprocessing
Data preprocessing played a crucial role in improving model accuracy:

Handling Missing Values: Filled missing categorical values with empty strings.
Feature Encoding:
One-hot encoding for categorical variables.
Binary encoding for certain categorical values.
Feature Scaling:
Standardized mileage, age, horsepower, and weight.
Log Transformation on Price:
Addressed skewness in the target variable.
Outlier Detection:
Examined outliers, particularly in mileage, and retained them as they were relevant.

Neural Network (NN) produced a 92%	accuracy rating. 
K-Nearest Neighbors (KNN, k=5)	produced a	94% accuracy rating.
