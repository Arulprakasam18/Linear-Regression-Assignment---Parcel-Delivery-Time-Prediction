# Linear-Regression-Assignment---Parcel-Delivery-Time-Prediction


# Delivery Time Estimation using Machine Learning

## Project Overview
This project focuses on estimating food delivery time using machine learning techniques. The dataset contains various features such as order details, item prices, delivery distance, and dasher availability. The goal is to build a predictive model that accurately estimates the time taken for an order to be delivered.

## Dataset Description
The dataset includes the following numerical features:
- `market_id`: Categorical ID for different markets.
- `total_items`: Total number of items in the order.
- `subtotal`: Total cost of the order before tax.
- `num_distinct_items`: Number of distinct items in the order.
- `min_item_price`: Minimum item price in the order.
- `max_item_price`: Maximum item price in the order.
- `total_onshift_dashers`: Number of dashers available.
- `total_busy_dashers`: Number of dashers currently delivering orders.
- `total_outstanding_orders`: Number of pending orders.
- `distance`: Distance from the restaurant to the customer.
- `isWeekend`: Whether the order was placed on a weekend (1) or not (0).

## Exploratory Data Analysis (EDA)
EDA was performed to understand feature distributions, detect outliers, and examine relationships between variables. Key visualizations include:
- **Histograms**: Show data distribution for numerical features.
- **Heatmap**: Displays correlation between features.
- **Residual Analysis**: Evaluates model performance by analyzing residuals.
- **Feature Importance**: Assesses the impact of different variables on delivery time.

## Model Training
### Train-Test Split
The dataset was split into training and testing sets:
```python
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
```

### Feature Selection & Engineering
Feature scaling and selection were performed to improve model performance. The final model was trained using **Linear Regression with RBF kernel**.

### Model Evaluation
The model was evaluated using key metrics:
- **Mean Absolute Error (MAE)**: 2.3394
- **Mean Squared Error (MSE)**: 10.3927
- **R-squared Score**: 0.8812

## Results & Inference
### Residual Analysis
Residuals were analyzed to check model fit. A normal distribution of residuals indicates good model performance.

### Coefficient Analysis
Coefficient values helped identify the impact of features on delivery time. The most influential features include **distance, total outstanding orders, and number of busy dashers**.

## Conclusion
The project successfully developed a predictive model for food delivery time estimation with high accuracy. Future improvements could include using deep learning models and real-time traffic data.

   ```

## Future Enhancements
- Incorporating **real-time traffic data**.
- Using **advanced deep learning models**.
- Implementing **geospatial analysis** for better distance estimation.

## Author
**Arulprakasam** 🚀

---
This README provides a structured overview of the project. Let me know if you need any modifications! 🔥
