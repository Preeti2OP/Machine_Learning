# Breast Cancer Prediction using k-Nearest Neighbors
## Overview
This project aims to predict breast cancer using the k-Nearest Neighbors (k-NN) algorithm. The dataset is processed, analyzed, and utilized to build a machine learning model for binary classification of breast cancer as either malignant (M) or benign (B).

##  Libraries and Tools
### scikit-learn: For model training, evaluation, and preprocessing.
### pandas: For data manipulation and analysis.
### matplotlib and seaborn: For data visualization.
### numpy: For numerical operations.
### Data Cleaning
The dataset used in this project is loaded and cleaned by removing unnecessary columns and handling missing values. The initial steps involve:

##  Loading the dataset:
https://www.kaggle.com/account/login?returnUrl=/datasets/yasserh/breast-cancer-dataset
The data is read from a CSV file.
The 'id' and 'Unnamed: 32' columns are dropped as they are not useful for prediction.

### Handling missing values:

The dataset is checked for missing values, and necessary steps are taken to handle them.
Data inspection:

A quick look at the first few rows of the dataset to understand its structure.
Feature Selection and Data Splitting
The features and target variables are separated for model training. The dataset is split into training and testing sets to evaluate the model's performance.

## Independent and dependent variables:

The feature variables (all columns except 'diagnosis') and the target variable ('diagnosis') are separated.
### Train-test split:

The data is split into training and testing sets using an 80-20 split.
### Data Preprocessing
Before training the model, the data is preprocessed to ensure it is in the correct format and scale:

## Label Encoding:

The categorical target variable ('diagnosis') is encoded into numerical values using LabelEncoder.
## Feature Scaling:

The feature variables are scaled using StandardScaler to standardize the data, ensuring all features contribute equally to the model.
## Model Training
The k-Nearest Neighbors (k-NN) algorithm is used for training the model. The steps involved are:

### Model initialization:

The KNeighborsClassifier from scikit-learn is used for classification.
### Model fitting:

The model is trained on the scaled training data.
### Model Evaluation
The trained model is evaluated on the test data to determine its accuracy and performance metrics:

## Predictions:

The model makes predictions on the scaled test data.
### Performance metrics:

Accuracy, confusion matrix, and classification report are used to evaluate the model's performance.
## Data Visualization
Correlation heatmaps are plotted to visualize the relationships between different features in the dataset.

##  User Input Model Testing
A function is created to test the model with user-provided input values:

### Input collection:

The function collects input values for the first four features from the user.
### Prediction:

The model makes predictions based on the user input, and the result is displayed as either malignant or benign.
