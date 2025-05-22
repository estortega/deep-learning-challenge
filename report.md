# Module 21

# Alphabet Soup’s Deep Learning Model

## Overview of the Analysis

The purpose of this analysis was to develop a binary classification model using deep learning to predict whether applicants funded by Alphabet Soup will be successful. Using historical application data provided by Alphabet Soup, a neural network was trained using TensorFlow and Keras to identify patterns in applicant features that correlate with a successful funding outcome.

The ultimate goal was to assist Alphabet Soup in making more informed decisions when awarding funding by accurately predicting which applicants are likely to succeed based on their historical profiles.

## Results

Data Preprocessing
Target Variable:
IS_SUCCESSFUL – This column indicates whether an applicant successfully used their funding. It serves as the binary target for the model (1 = successful, 0 = not successful).
Feature Variables:
All other variables in the dataset except for identifiers were used as features, including:
Categorical variables: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, INCOME_AMT
Numeric variables: ASK_AMT
These features were encoded using one-hot encoding and normalized as needed.
Removed Variables:
EIN – A unique identifier with no predictive value.
NAME – Organization name, likely to cause overfitting or introduce noise.
Compiling, Training, and Evaluating the Model
Model Architecture:
Input layer: Based on 43 input features after encoding.
Hidden Layers:
1st Hidden Layer: 80 neurons, ReLU activation
2nd Hidden Layer: 30 neurons, ReLU activation
Dropout Layer: Dropout rate of 0.3 to reduce overfitting
Output Layer: 1 neuron with sigmoid activation for binary classification
Compilation Settings:
Optimizer: Adam
Loss Function: BinaryCrossentropy
Metrics: Accuracy
Model Performance:
Final validation accuracy was approximately 73–75%
The model did not consistently achieve the target performance threshold of 75% accuracy
Steps Taken to Improve Model Performance:
Tuned number of layers and neurons
Introduced dropout layers to reduce overfitting
Adjusted batch size and epochs
Evaluated impact of different activation functions
Pruned features with low correlation or high cardinality
## Summary

The deep learning model achieved modest success with an accuracy close to the 75% target, but failed to consistently meet it. While neural networks are powerful, they may not always be the most efficient approach for structured, tabular datasets such as this.

Recommendation:
A more effective approach for this classification task could be to use ensemble models, such as:

Random Forest
Gradient Boosted Trees (XGBoost)
These models often perform better on structured data and offer improved interpretability and shorter training times. In future iterations, applying traditional machine learning techniques along with feature selection and hyperparameter tuning may yield higher performance and better generalizability.