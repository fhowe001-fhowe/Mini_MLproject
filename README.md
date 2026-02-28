# Mini_MLproject
A mini prediction project using jupyter notebook. 

## Project Overview

This project explores whether we can predict the likelihood of an aviation accident being fatal based on historical accident data.

The objective was to build a machine learning model that classifies accidents into Fatal or Non-Fatal, and to identify which factors most significantly influence fatal outcomes.

## Data Preparation

We selected key features from the dataset, which we believed contributes to the likelihood of the fatality of an accident. The key features selected are:

- Event Date

- Aircraft Make

- Aircraft Model

- Weather Condition

- Total Fatal Injuries

Key preprocessing steps:

1) Converted event dates into seasons

2) Transformed total fatal injuries into a binary target variable (Fatal vs Non-Fatal)

3) Replaced missing weather values with "UNK"

4) Standardised categorical values (e.g., uppercase formatting)

## Exploratory Data Analysis

We analysed fatality trends across:

- Aircraft Make

- Aircraft Model

- Weather Conditions

- Season

This helped identify patterns and potential predictors before modelling.

## Machine Learning Approach

We implemented a Random Forest classifier to predict accident fatality.

Reasons for choosing Random Forest:

- Strong performance on structured tabular data

- Reduced overfitting compared to single decision trees

- Ability to measure feature importance

Since most features were categorical, we applied One-Hot Encoding to convert them into numerical format suitable for machine learning.

We trained and evaluated models using different numbers of trees (n_estimators = 10 and 100) and refined the model to improve performance.

## Results

The final model achieved approximately 91.6% accuracy in predicting whether an accident would be fatal.

Feature importance analysis indicated that:

- Weather condition

- Month/Season

- Aircraft Make

were significant contributors to fatality prediction.

## Limitations

Accuracy alone may not fully reflect model performance (class imbalance considerations).

The dataset may contain reporting inconsistencies.

External factors not included in the dataset could influence outcomes.

## Conclusion

The results suggest that fatal accident likelihood can be predicted with reasonable accuracy using structured accident data. Key environmental and aircraft-related factors appear to significantly influence fatal outcomes.
