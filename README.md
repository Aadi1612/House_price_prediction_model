# House Price Prediction Project

## Introduction
This project aims to predict house prices using machine learning techniques. The dataset used for this project contains various features of houses such as their size, location, number of rooms, etc. This repository contains code for training and evaluating three different regression models: Linear Regression, RandomForestRegressor, and GradientBoostingRegressor. The goal is to predict a target variable based on a set of features.

## Requirements
To run this project, you need to have Python installed on your system along with the following libraries:
- pandas
- seaborn
- matplotlib
- numpy
- scikit-learn

You can install these libraries using pip:
```
pip install pandas seaborn matplotlib numpy scikit-learn
```

## Usage
1. Clone this repository to your local machine.
2. Make sure you have Python and the required libraries installed.
3. Open the Jupyter Notebook file `house_price_prediction.ipynb` in your Jupyter Notebook environment.
4. Run the cells in the notebook to execute the code step by step.
5. Follow the comments in the code for better understanding.

## Data
The dataset used in this project contains the following columns:
- **SalePrice**: The sale price of the house (target variable)
- **MSZoning**: The zoning classification of the property
- **Street**: Type of road access to the property
- **HeatingQC**: Heating quality and condition
- **TotRmsAbvGrd**: Total rooms above grade (does not include bathrooms)
- **GrLivArea**: Above grade (ground) living area square feet
- **1stFlrSF**: First Floor square feet
- **GarageArea**: Size of garage in square feet
- **FullBath**: Full bathrooms above grade
- **OverallQual**: Overall material and finish quality
- **YearRemodAdd**: Remodel date (same as construction date if no remodeling or additions)

## Preprocessing
- Null values in certain columns were handled using appropriate strategies (e.g., mean imputation, constant imputation).
- Categorical variables were one-hot encoded to convert them into numerical format.
- Feature selection was performed based on correlation analysis with the target variable.

## Model Training and Evaluation
Various machine learning algorithms were trained and evaluated using the preprocessed data. The model with the highest performance was selected for making predictions.

## Results
After training and evaluating the models, the following results were obtained:

Linear Regression:
MAE (Mean Absolute Error): 54384.24
MSE (Mean Squared Error): 4547579713.20
RMSE (Root Mean Squared Error): 67435.75

RandomForestRegressor:
MAE: 53412.51
MSE: 4852419649.39
RMSE: 69659.31

GradientBoostingRegressor:
MAE: 11454.03
MSE: 254604964.28
RMSE: 15956.35
Conclusion

## Conclusion
Based on the evaluation metrics, here are the conclusions:

GradientBoostingRegressor significantly outperforms the other two models, achieving much lower MAE, MSE, and RMSE values. It provides the most accurate predictions among the models tested.

RandomForestRegressor performs better than Linear Regression but not as well as GradientBoostingRegressor. While it offers decent performance, it falls short compared to the boosting model.

Linear Regression has the highest error metrics among the three models, indicating it performs the worst in this comparison. It may not be the ideal choice for this particular prediction task.
In conclusion, this project demonstrates the use of machine learning techniques to predict house prices based on various features. The trained model can be used by real estate agents, homeowners, or buyers to estimate the value of a property. 

