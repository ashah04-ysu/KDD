# KDD

## Overview
This code is for training a machine learning model to predict the risk of heart disease in patients. The code uses the CardiologyN-Wekat dataset, which contains data on patients such as their age, chest pain type, and heart rate, and whether or not they have heart disease. The code uses two classifiers: Decision Tree and Extra Trees Classifier, and it evaluates the performance of these classifiers using cross-validation and the accuracy score. The code also performs feature selection and feature importances analysis.

## Steps
1. Import necessary libraries (numpy, pandas, sklearn)
2. Load the CardiologyN-Wekat dataset into a pandas dataframe and check the value counts for the target column ('class')
3. Normalize the dataset using MinMaxScaler
4. Split the normalized dataset into features (X) and target (y)
5. Train a Decision Tree Classifier and evaluate its performance using cross-validation and accuracy score
6. Train an Extra Trees Classifier and evaluate its performance using cross-validation and accuracy score
7. Perform feature selection using SelectKBest with chi2 as the scoring function and choose the top 7 features
8. Train the Decision Tree and Extra Trees Classifier on the selected features and evaluate their performance using cross-validation and accuracy score
9. Plot the feature importances from the Extra Trees Classifier to visualize the most important features
10. Train the Extra Trees Classifier on the final selected features (thal, #colored-vessels, chest-pain-type, peak, maximum-heart-rate, angina, age) and evaluate its performance using cross-validation and accuracy score.
## Conclusion
Based on the results, the Extra Trees Classifier performed best with the highest mean accuracy score and lowest standard deviation. The most important features for predicting heart disease risk were found to be thal, #colored-vessels, chest-pain-type, peak, maximum-heart-rate, angina, and age.
