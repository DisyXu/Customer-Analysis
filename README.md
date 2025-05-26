# Customer Segmentation Using RFM and K-Means Clustering

## 📌 Project Overview

This project performs customer segmentation using RFM (Recency, Frequency, Monetary) analysis combined with unsupervised K-Means clustering to identify high-value customer groups for targeted marketing.

## 📁 Data Source

- `customer_data.csv`: customer demographic & ID info
- `sales_data.csv`: transaction details (invoice, amount, date, etc.)

## ⚙️ Analysis Process

1. **Data Merging & Cleaning**
   - Merged customer and sales data
   - Removed missing or inconsistent records

2. **RFM Calculation**
   - Recency: days since last purchase
   - Frequency: number of purchases
   - Monetary: total spending per customer

3. **RFM Scoring**
   - Customers scored using quartiles (1–4)
   - Segment labels based on custom logic

4. **KMeans Clustering**
   - Scaled RFM values
   - K=4 clusters trained
   - Clusters interpreted with business labels

## 📊 Results

| Cluster Label             | Characteristics                                | Strategy Suggestion              |
|---------------------------|------------------------------------------------|----------------------------------|
| High Value Customer       | Spends a lot, needs retention strategy         | VIP programs / loyalty rewards   |
| Mid-High Spending Customer| Infrequent but valuable                        | Encourage reactivation           |
| Regular Customer          | Average spending and recency                   | Incentivize further purchases    |
| Dormant Customer          | Inactive and low value                         | Optional targeting or ignore     |

## 📁 Output

- 📄 `high_value_customers.csv`: List of top-tier customers for marketing use
- 📈 Visualizations: RFM scores, cluster sizes, scatter plots

## 🛠 Tools Used

- Python (Pandas, Seaborn, Matplotlib, scikit-learn)
- Jupyter Notebook

## 📚 Data Source (APA Citation)

Khanh Lai. (2023). *Mini Project - Data Analytics with SQL and Python* [Dataset]. Kaggle. https://www.kaggle.com/code/khanhlai03/mini-project-data-analytics-with-sql-and-python

Note: This dataset is intended for educational and analytical purposes.

