# 🚗 Car Price Prediction using Machine Learning

A machine learning project that predicts the selling price of used cars based on features such as present price, car age, driven kilometers, fuel type, selling type, transmission, and previous ownership.

## 📌 Project Overview

The aim of this project is to build a regression model that can estimate the selling price of a used car from its characteristics.

The project covers the complete machine learning workflow:

- Data loading and inspection
- Data cleaning
- Exploratory Data Analysis
- Feature engineering
- Categorical encoding
- Train-test split
- Model training
- Model evaluation
- Feature importance
- Actual vs predicted analysis
- Manual price prediction
- Input validation

## 🗂️ Dataset

The dataset contains information about used cars, including:

| Feature | Description |
|---|---|
| `Car_Name` | Name of the car |
| `Year` | Manufacturing year |
| `Selling_Price` | Selling price |
| `Present_Price` | Present price |
| `Driven_kms` | Kilometers driven |
| `Fuel_Type` | Petrol, Diesel or CNG |
| `Selling_type` | Dealer or Individual |
| `Transmission` | Manual or Automatic |
| `Owner` | Number of previous owners |

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## 🔍 Data Preprocessing

The following steps were performed:

1. Checked for missing values
2. Checked and removed duplicate rows
3. Created a `Car_Age` feature
4. Removed unnecessary columns
5. Encoded categorical variables using one-hot encoding
6. Split the dataset into training and testing sets

The dataset was divided into:

- **80% Training**
- **20% Testing**

## 🤖 Machine Learning Models

Two regression models were implemented:

### Random Forest Regressor

Used as the initial regression model for predicting car selling prices.

### Gradient Boosting Regressor

Used as the final model after comparing its performance with Random Forest.

## 📊 Model Performance

| Model | MAE | MSE | RMSE | R² |
|---|---:|---:|---:|---:|
| Random Forest | 1.47 | 12.32 | 3.51 | 0.52 |
| Gradient Boosting | 1.21 | 8.04 | 2.84 | 0.69 |

The Gradient Boosting model achieved an R² score of approximately **0.69** on the test set used in this project.

## 📈 Visualizations

The project includes:

- Selling Price Distribution
- Present Price vs Selling Price
- Car Age vs Selling Price
- Feature Importance
- Actual vs Predicted Prices

## 🔮 Manual Price Prediction

The final model allows users to enter car details manually:

```text
Present Price
Driven Kilometers
Number of Previous Owners
Car Age
Fuel Type
Selling Type
Transmission
