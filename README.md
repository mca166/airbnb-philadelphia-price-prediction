# Machine Learning-Based Airbnb Price Prediction in the Philadelphia Market

This project predicts Airbnb nightly prices in the Philadelphia short-term rental market using listing, host, location, and review-score features.

## Project Motivation

This project is motivated by real-world Airbnb pricing decisions near Collingdale, Pennsylvania, which is close to Philadelphia. The goal is to understand which listing features are most related to nightly price and whether structured Airbnb data can be used to predict prices.

## Dataset

The dataset used in this project is the Philadelphia Airbnb Master Dataset obtained from Doorstep Analytics. The uploaded file `philly_master.csv` contains listing-level information such as room type, bedrooms, bathrooms, guest capacity, host features, review counts, rating scores, location variables, and nightly price.

## Methods

The project includes:

- Data cleaning and target variable preparation
- Log transformation of nightly price
- Exploratory data analysis
- One-hot encoding of categorical variables
- Manual feature scaling using training data only
- Train/test split using scikit-learn
- Baseline mean model
- Linear regression implemented from scratch with NumPy
- Ridge regression implemented from scratch with NumPy
- Model evaluation using MAE, RMSE, and R²

## Main Results

The best overall model was Ridge Regression with alpha = 10. It achieved an R² score of about 0.67 on the log-transformed price target and an average prediction error of about $63 per night.

## Files

- `Airbnb_price_prediction.ipynb`: main notebook with data cleaning, modeling, and evaluation
- `philly_master.csv`: dataset used for the project
- `model_results.csv`: model performance table
- `ridge_predictions.csv`: actual vs. predicted prices from the best model
- `top_ridge_features.csv`: top features from the ridge regression model
- `.png` files: figures used for analysis and reporting

## Tools Used

- Google Colab
- Python
- pandas
- NumPy
- matplotlib
- seaborn
- scikit-learn
- Overleaf / LaTeX
