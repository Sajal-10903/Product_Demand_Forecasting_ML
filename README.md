# Product Demand Forecasting using Machine Learning

## Overview
Accurate demand forecasting is critical for effective inventory management and supply chain planning.  
This project focuses on predicting product demand (quantity sold) using historical order, pricing, and temporal data with regression-based machine learning models.

---

## Objective
The objective of this project is to build and evaluate regression models that can predict product demand based on historical sales patterns, pricing, discounts, and time-related features.

---

## Dataset
The dataset contains order-level retail transaction data with the following relevant attributes:
- Order Date
- Ship Mode
- Order Priority
- Customer Segment
- Region
- Product Category and Sub-Category
- Unit Price
- Discount
- Quantity (Target Variable)

The target variable for this project is **Quantity**, representing the number of units sold for each order.

---

## Tools & Technologies
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook

---

## Methodology
The project follows a structured machine learning workflow:

1. **Data Preparation**
   - Selected relevant order, product, and pricing features
   - Converted date fields into datetime format
   - Removed non-informative identifiers

2. **Feature Engineering**
   - Extracted temporal features such as year, month, day, and day of week from order dates
   - Applied one-hot encoding to categorical variables

3. **Model Building**
   - Linear Regression used as a baseline regression model
   - Random Forest Regressor used to capture non-linear demand patterns

4. **Model Evaluation**
   - Evaluated models using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE)
   - Compared baseline and ensemble model performance

5. **Interpretability**
   - Analyzed feature importance from the Random Forest model to identify key demand drivers

---

## Results & Key Insights
- Random Forest outperformed Linear Regression by better capturing non-linear relationships in demand data.
- Product category, unit price, discount levels, and temporal features significantly influenced demand.
- Temporal patterns such as month and day of week contributed to variations in sales quantity.

---

## Business Impact
The insights from this project can help businesses:
- Improve inventory planning and stock management
- Anticipate demand fluctuations across products and time periods
- Reduce overstocking and stock-out risks

---

## Conclusion
This project demonstrates how regression-based machine learning models can be applied to retail sales data for demand forecasting. By combining feature engineering, model evaluation, and interpretability, the project provides both predictive accuracy and actionable business insights.

---

## Future Enhancements
- Incorporate lag-based features for stronger time dependency modeling
- Perform hyperparameter tuning for regression models
- Extend the approach to store-level or category-level forecasting
