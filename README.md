# Weather Prediction Using Ensemble Classifiers

## Project Overview

This project involves the development of a predictive model to estimate whether it will rain the next day. The project utilizes an ensemble of RandomForest and GradientBoosting classifiers, evaluated and optimized using grid search. The dataset used is sourced from [Kaggle](https://www.kaggle.com/datasets/nikhil7280/weather-type-classification).

## Implementation Steps

### Data Loading and Preprocessing

1. Load the dataset.
2. Drop any missing values.
3. Encode categorical features using `LabelEncoder`.
4. Split the dataset into training (70%) and testing (30%) sets using stratified sampling to ensure class balance.

### Model Training and Optimization

1. Train individual models: RandomForest and GradientBoosting.
2. Create an ensemble classifier using soft voting.
3. Define parameter grids for both classifiers for grid search.
4. Perform grid search with 10-fold cross-validation to find the best hyperparameters.
5. Select the best model based on cross-validation results.

### Model Evaluation

1. Evaluate the model's accuracy on both training and testing sets.
2. Print classification reports and confusion matrices for both sets.
3. Assess potential overfitting by comparing cross-validation scores on training and testing sets.
4. Calculate confidence intervals for the test set accuracy using normal approximation.

### Plots and Visualization

1. Plot learning curves to visualize training and validation scores over different training set sizes.
2. Plot validation curves to visualize the effect of different hyperparameters on model performance.
