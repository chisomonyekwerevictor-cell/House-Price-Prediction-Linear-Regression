# House Price Prediction using Linear Regression

## Project Overview
This project builds a baseline machine learning model to predict house prices
using Linear Regression. The focus is on following a correct end-to-end ML
workflow rather than optimizing for the best possible score.

## Dataset
The dataset contains housing features such as:
- Property size (living area, lot size)
- Quality and condition
- Basement and garage information
- Room counts and construction year
Target variable: SalePrice

## Data Cleaning & Preprocessing
Key preprocessing decisions include:
- Dropping identifier columns that carry no predictive meaning
- Handling missing values based on feature context:
  - Measurement-based features filled with median
  - Non-existent features filled with zero
- Verifying the dataset contains no missing values before modeling

## Feature Selection
Only core numeric features were selected to:
- Reduce noise
- Improve interpretability
- Create a stable baseline model

Categorical features were intentionally excluded at this stage.

## Model
- Algorithm: Linear Regression
- Train/Test split: 80/20
- Evaluation metrics:
  - RMSE
  - R² score

## Results
- RMSE: ~$30,301.09
- R² Score: ~0.83

The model performs well on average-priced homes but struggles with extreme values.

## Model Interpretation
Model coefficients were analyzed to understand feature importance.
Feature scaling was applied to compare coefficients fairly and confirm
the correctness of the implementation.

## Key Learnings
- Data understanding is more important than model choice
- Linear models are interpretable but limited
- Proper preprocessing is critical for reliable results

## Next Steps
- Decision Tree Regression
- Ensemble methods
- Classification projects (spam or fraud detection)

## Requirements
pandas  
numpy  
scikit-learn
