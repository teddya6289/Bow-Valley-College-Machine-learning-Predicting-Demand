# Summary of the Model Presentation

## 1. Dataset & Preprocessing

- Dataset includes features like Hour of day, Gender, User Type, Temperature, Humidity, Wind Speed, Solar Energy, etc.

**Data preprocessing involved:**

- SimpleImputer for missing values

- StandardScaler for numerical variables

- One-Hot Encoding for categorical variables

## 2. Model Development
ElasticNet Regression was chosen for its ability to:
Prevent overfitting using Lasso (shrinks irrelevant feature coefficients to zero)
Control large coefficients using Ridge (penalizes high values).
Data was split into 80% training and 20% testing sets.

## 3. Key Insights

**Gender and User Type are the strongest predictors of bike demand.**

- A 1% change in these features leads to over 1000% impact on bike demand.

## 4. Model Performance

- R² = 0.818 → Model explains 81.8% of bike demand variation.

- Mean Prediction Error = 18.8

- Percentage Error = 6.38% → Prediction close to actual demand.

## 5. Business Recommendations

- Average demand = 277 bikes/day

- Rush hour demand = up to 993 bikes

- **Charging point requirement:** 1 station for every 5 bikes → 55 charging stations needed.

## 6. Final Decision

- Install 55 charging stations to meet both normal and peak demand efficiently.
Find attached the file [`Machine Learning Script`](Bike_Demand_prediction.ipynb)
