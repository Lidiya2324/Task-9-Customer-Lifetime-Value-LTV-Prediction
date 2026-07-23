# Customer Lifetime Value (LTV) Prediction and Customer Segmentation

## Project Overview

Customer Lifetime Value (LTV) is a key business metric that estimates the total revenue a customer is expected to generate throughout their relationship with a business. This project develops a machine learning model to predict Customer Lifetime Value using historical online retail transaction data and segments customers based on their predicted value to support data-driven business decisions.

The project follows a complete data analytics and machine learning workflow, including data cleaning, exploratory data analysis (EDA), feature engineering, predictive modeling, customer segmentation, and business visualization.

---

## Business Objective

The primary objectives of this project are to:

* Predict Customer Lifetime Value (LTV) using customer purchasing behavior.
* Identify high-value customers for targeted retention strategies.
* Segment customers into High, Medium, and Low Value groups.
* Generate business insights that support customer relationship management and marketing decisions.

---

## Dataset

* **Dataset:** Online Retail Dataset
* **Source:** UCI Machine Learning Repository
* **Cleaned Transactions:** 392,693
* **Unique Customers:** 4,338
* **Countries:** 37

The dataset contains historical online retail transactions, including invoice details, products, quantities, prices, customer IDs, and purchase dates.

---

## Tools and Technologies

* Python
* Jupyter Notebook
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Linear Regression

---

## Project Workflow

### 1. Data Cleaning

* Removed duplicate records.
* Removed cancelled transactions.
* Removed missing customer IDs.
* Removed invalid quantity and unit price values.
* Created the Revenue feature.

### 2. Exploratory Data Analysis (EDA)

* Customer spending analysis.
* Purchase frequency analysis.
* Revenue distribution.
* Top customers by revenue.
* Country-wise sales analysis.
* Correlation analysis.
* Sales trend visualization.

### 3. Feature Engineering

Created customer-level features including:

* Recency
* Frequency
* Monetary (RFM)
* Average Order Value
* Total Quantity Purchased
* Unique Products Purchased
* Customer Lifetime
* Average Basket Size

### 4. Machine Learning

* Prepared customer-level dataset.
* Scaled input features.
* Trained a Linear Regression model.
* Predicted Customer Lifetime Value (LTV).

### 5. Customer Segmentation

Customers were segmented into:

* High Value
* Medium Value
* Low Value

using quantile-based segmentation (`qcut`).

### 6. Final Visualizations

The project includes visualizations for:

* Predicted LTV Distribution
* Customer Distribution by Segment
* Average Predicted LTV by Segment
* Top 10 Customers by Predicted LTV
* Customer Recency vs Predicted LTV

---

## Key Findings

* Customer purchasing behavior strongly influences future customer value.
* Monetary value and Total Quantity were the most influential features in predicting Customer Lifetime Value.
* Customer value is highly skewed, with a relatively small number of customers contributing a significant portion of future revenue.
* Customer segmentation provides valuable insights for personalized marketing, customer retention, and resource allocation.

---

## Project Structure

```text
Customer-Lifetime-Value-Prediction/
│
├── LTV_Prediction_Project.ipynb
├── Customer_LTV_Predictions.csv
├── Customer_LTV_Report.pdf
├── README.md
│
├── outputs/
│   └── charts/
│       ├── ltv_distribution.png
│       ├── customer_segments.png
│       ├── average_ltv_by_segment.png
│       ├── top10_customers.png
│       └── recency_vs_ltv.png
│
└── dataset/
```

---

## Future Improvements

* Evaluate additional regression models such as Random Forest Regressor and XGBoost Regressor.
* Apply hyperparameter tuning to improve prediction accuracy.
* Address negative LTV predictions by using models that naturally constrain outputs or by applying target transformations.
* Deploy the model as an interactive web application or business dashboard.

---

## Author

**Lidiya Mitiku**

GitHub: https://github.com/Lidiya2324

LinkedIn: https://www.linkedin.com/in/lidiya-mitiku-10b816189/
