# ☀️ Solar Efficiency Prediction

Predict the efficiency of solar panels using machine learning!

## Overview
This project uses an XGBoost regression model to predict the efficiency of solar panels based on provided features. The workflow includes data preprocessing, model training, validation, and generating predictions for submission.

## Features
- Automated preprocessing of categorical features
- Robust model training with XGBoost
- Validation with RMSE-based scoring
- Easy-to-use prediction and submission pipeline

## Project Structure
```
├── main.py                # Main script for training and prediction
├── train.csv              # Training data
├── test.csv               # Test data
├── sample_submission.csv  # Submission format template
├── submission.csv         # Generated predictions
├── model.pkl              # Saved trained model
└── README.md              # Project documentation
```

## Setup
1. **Clone the repository**
2. **Install dependencies**
   ```bash
   pip install pandas numpy scikit-learn xgboost
   ```
3. **Place your data files** (`train.csv`, `test.csv`, `sample_submission.csv`) in the project directory.

## Usage
Run the main script to train the model and generate predictions:
```bash
python main.py
```
- The script will print a validation score.
- Predictions will be saved to `submission.csv`.
- The trained model will be saved as `model.pkl`.

## Model Details
- **Algorithm:** XGBoost Regressor
- **Validation:** 20% hold-out set, RMSE-based score
- **Categorical Handling:** Label Encoding with safe handling of unseen categories

## Customization
- Adjust model parameters in `main.py` for experimentation.
- Replace data files with your own for new predictions.