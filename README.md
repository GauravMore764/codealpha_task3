Car Price Prediction using Machine Learning

A machine learning project that predicts the selling price of used cars based on features such as present price, car age, driven kilometers, fuel type, transmission, selling type, and previous ownership.

Features
Data cleaning and preprocessing
Exploratory Data Analysis (EDA)
Feature engineering
Categorical data encoding
Train-test splitting
Random Forest Regression
Gradient Boosting Regression
Model evaluation
Feature importance visualization
Actual vs Predicted visualization
Manual car price prediction
Input validation for invalid values
Dataset

The dataset contains 301 car records with the following features:

Feature	Description
Car_Name	Name of the car
Year	Manufacturing year
Selling_Price	Selling price of the car
Present_Price	Current price of the car
Driven_kms	Kilometers driven
Fuel_Type	Fuel type
Selling_type	Dealer or Individual
Transmission	Manual or Automatic
Owner	Number of previous owners
Technologies Used
Python
Pandas
NumPy
Matplotlib
Scikit-learn
Jupyter Notebook
Machine Learning Models
Random Forest Regressor

Initial regression model used for predicting car selling prices.

Gradient Boosting Regressor

A second regression model was trained and evaluated on the same test data.

Model Performance
Model	MAE	MSE	RMSE	R²
Random Forest	1.47	12.32	3.51	0.52
Gradient Boosting	1.21	8.04	2.84	0.69

Gradient Boosting achieved the higher R² and lower error metrics on the test split used in this project.

Data Preprocessing

The following steps were performed:

Checked for missing values
Checked and removed duplicate rows
Created a Car_Age feature
Removed unnecessary columns
Encoded categorical variables using one-hot encoding
Split the data into training and testing sets

The dataset was split into:

80% Training Data
20% Testing Data
Visualizations

The project includes:

Selling Price Distribution
Present Price vs Selling Price
Car Age vs Selling Price
Feature Importance
Actual vs Predicted Prices
Manual Prediction

The final model allows users to manually enter:

Present Price
Driven Kilometers
Number of Previous Owners
Car Age
Fuel Type
Selling Type
Transmission

The model then predicts the estimated selling price in lakhs.

Example
Enter present price: 5.59
Enter kilometers driven: 27000
Enter number of previous owners: 0
Enter car age: 5
Enter fuel type: Petrol
Enter selling type: Dealer
Enter transmission: Manual

Predicted Selling Price: 4.01 lakhs
Input Validation

The manual prediction system validates the entered values.

Input	Valid Range
Present Price	0.32 – 92.60 lakhs
Driven Kms	500 – 500000 km
Previous Owners	0 – 3
Car Age	2 – 21 years
Fuel Type	Petrol / Diesel
Selling Type	Dealer / Individual
Transmission	Manual / Automatic

Invalid values are rejected and an error message is displayed instead of making a prediction.

Project Structure
Car-Price-Prediction/
│
├── car data.csv
├── Car_Price_Prediction.ipynb
└── README.md
Installation

Install the required libraries:

pip install pandas numpy matplotlib scikit-learn
How to Run
Clone the repository.
Open Car_Price_Prediction.ipynb in Jupyter Notebook or VS Code.
Make sure car data.csv is in the same project folder.
Run the notebook cells in order.
Use the final cell to enter car details and generate a predicted selling price.
Conclusion

This project demonstrates a complete machine learning workflow for used-car price prediction, from data preprocessing and exploratory analysis to model training, evaluation, visualization, and manual prediction.
