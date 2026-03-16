# House Price Prediction Project

This project focuses on predicting house prices using machine learning techniques, specifically the XGBoost algorithm. The dataset used is the California housing dataset, which contains various features related to housing districts.

## Project Overview
The goal of this project is to build a regression model that can accurately predict the median house value for districts in California based on features such as location, income, housing age, and more.

## Dataset
The dataset consists of 20,640 rows and 10 columns:
- longitude: Geographic coordinate
- latitude: Geographic coordinate
- housing_median_age: Median age of houses in the district
- total_rooms: Total number of rooms
- total_bedrooms: Total number of bedrooms
- population: District population
- households: Total number of households
- median_income: Median income of residents
- median_house_value: Target variable (house price)
- ocean_proximity: Proximity to the ocean (categorical)

## Data Preprocessing
- Checked for missing values (total_bedrooms had 207 missing values)
- Filled missing values with median
- Checked for duplicates (none found)
- Converted categorical variable 'ocean_proximity' to numerical using one-hot encoding
- Explored data distribution and correlations using visualizations

## Model Building
- Split data into training (80%) and testing (20%)
- Used XGBoost Regressor for prediction
- Applied feature name sanitization for XGBoost compatibility

## Model Evaluation
- R² Score: 0.839
- Mean Absolute Error: 30,167

## Technologies Used
- Python
- Pandas (data manipulation)
- NumPy (numerical operations)
- Matplotlib & Seaborn (visualization)
- Scikit-learn (data splitting)
- XGBoost (modeling)
- Pickle (model saving)

## How to Use
1. Clone the repository:
   git clone https://github.com/hassanelsharkawy-ML/House_price_prediction_ML.git

2. Open the Jupyter notebook file:
   House_price_prediction.ipynb

3. Run all cells to see the full analysis and model training.

## Model Saving
The trained model is saved as 'house_price_model.pkl' for future use.

## Author
hassanelsharkawy-ML

## License
This project is licensed under the MIT License.
