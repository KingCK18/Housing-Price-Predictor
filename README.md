# House Price Prediction

This project builds a machine learning model to predict residential housing prices using structured property features from the Kaggle *House Prices: Advanced Regression Techniques* dataset. The project was completed as part of the **AITP Fall 2025 Dual-Supplied Applied Machine Learning program**.

## Project Overview
The goal of this project is to predict home sale prices based on features describing size, quality, age, and location. Emphasis was placed on data cleaning, feature engineering, and interpretability rather than model complexity.

## Dataset
- Source: Kaggle – House Prices: Advanced Regression Techniques
- Training samples: 1,460
- Target variable: `SalePrice`
- Feature types: Numerical and categorical housing attributes

## Methods
### Exploratory Data Analysis
- Identified right-skewed distribution of sale prices
- Analyzed correlations between size, quality, and price
- Investigated missing value patterns

### Data Cleaning
- Dropped features with excessive missing values
- Filled missing numerical values using median or zero
- Filled categorical missing values using `"None"`
- Removed non-informative identifiers

### Feature Engineering
- Total square footage
- Total bathrooms
- House age and years since remodel
- Binary indicators for major amenities
- Quality × size interaction feature

### Modeling
- Train/validation split (80/20)
- Log-transformed target variable
- Models:
  - Linear Regression
  - Ridge Regression
- Evaluation metric: Root Mean Squared Error (RMSE)

## Results
- Linear Regression RMSE ≈ 0.134
- Ridge Regression RMSE ≈ 0.134
- Regularization did not significantly improve performance, indicating effective feature engineering and limited overfitting.

## Tools Used
- Python
- pandas
- NumPy
- scikit-learn
- matplotlib

## Future Work
- Train non-linear models such as Random Forest or XGBoost
- Perform systematic hyperparameter tuning
- Incorporate external geospatial data
- Expand model explainability for client-facing insights

## Author
Christian Kirby  
Duke University – Computer Science (AI/ML Concentration)
