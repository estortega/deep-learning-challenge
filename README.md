# Alphabet Soup Charity Optimization

This project uses a deep learning model to help the Alphabet Soup Foundation predict whether applicants will be successful if funded. It is part of a binary classification challenge focused on optimizing funding decisions using historical application data.

## 🚀 Project Overview

- **Goal:** Predict the success of nonprofit funding applicants.
- **Model:** Deep neural network using TensorFlow/Keras.
- **Data:** Historical application data from Alphabet Soup Foundation.
- **Output:** A trained model saved as `AlphabetSoupCharity_Optimization.h5`.

## 🧠 Technologies Used

- Python
- Pandas & NumPy
- Scikit-learn
- TensorFlow / Keras
- Jupyter Notebook

## 📊 Model Architecture

- **Input Layer:** Features selected after preprocessing (one-hot encoding, dropping unnecessary columns).
- **Hidden Layers:** 2 dense layers with ReLU activation and dropout.
- **Output Layer:** 1 neuron with sigmoid activation for binary classification.

## 📈 Performance

- **Accuracy:** ~75% (baseline may vary based on preprocessing and tuning).
- Additional metrics like precision/recall/F1-score can be added for more insight.

## 🧪 Future Improvements

- Hyperparameter tuning (layer size, dropout rate, batch size).
- Try other models: Random Forest, XGBoost for comparison.
- Add confusion matrix & ROC curve for evaluation.
