# Disease-Prediction--Machine-learning
# Lung Cancer Prediction Using Python

This project aims to predict lung cancer presence using a machine learning model based on a small survey dataset. The dataset includes various features such as demographic, lifestyle, and health-related factors to build a predictive model.

## Dataset Description

The dataset, **mini survey lung cancer.csv**, contains the following columns:

- **GENDER**: Categorical (M for Male, F for Female)
- **AGE**: Integer, representing the age of the individuals.
- **SMOKING**: 1 for No, 2 for Yes
- **ANXIETY**: 1 for No, 2 for Yes
- **CHRONIC DISEASE**: 1 for No, 2 for Yes
- **ALCOHOL CONSUMING**: 1 for No, 2 for Yes
- **SHORTNESS OF BREATH**: 1 for No, 2 for Yes
- **CHEST PAIN**: 1 for No, 2 for Yes
- **LUNG_CANCER**: Target variable (Yes or No)

## Project Workflow

1. **Data Preprocessing**: 
   - Replaced all binary variables (2 for Yes, 1 for No) with more readable labels ('Yes' and 'No').
   - Categorized individuals into age groups: "Middle" for ages less than 65, and "Old" for ages 65 and above.
   - Converted categorical variables like GENDER and LUNG_CANCER into numerical values for machine learning models.

2. **Exploratory Data Analysis (EDA)**:
   - Created bar plots to analyze the relationships between smoking and lung cancer, as well as alcohol consumption and lung cancer, to visually explore any potential correlations.

3. **Modeling**: 
   - Split the dataset into 80% training and 20% testing data.
   - Performed 5x cross-validation on the training set to validate model performance.
   - Tested the trained model on the 20% test data to evaluate its generalization to unseen data.
   - Evaluated models using performance metrics such as accuracy, precision, recall, and F1-score.

## Results

- **Cross-validation**: The cross-validation results provided insights into how well the model performs on different splits of the training data. The accuracy from cross-validation was consistent across most folds, giving confidence in the model’s robustness.
  
- **Test Results**: When tested on the 20% test data, the model's performance was comparable to the cross-validation results, though slight differences were observed. This indicates that the model generalizes reasonably well to new data.

- **Comparison of Cross-validation and Test**: The model showed a small performance dip when tested on the test data compared to cross-validation, suggesting that it can predict new data with reasonable confidence but may still benefit from further tuning.

## Future Work

- **Model Improvement**: Future work could include trying different algorithms such as Random Forest, SVM, or Gradient Boosting to improve predictive performance.
- **Hyperparameter Tuning**: Explore hyperparameter tuning techniques like Grid Search or Random Search to fine-tune the model for better results.
- **Feature Engineering**: Additional features could be engineered based on domain knowledge to improve prediction accuracy.
- **Deep Learning Models**: Implement a deep learning model (e.g., Neural Networks) to see if it outperforms traditional machine learning approaches.

