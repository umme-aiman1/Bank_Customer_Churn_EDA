# Bank Customer Churn Analysis

##  Project Overview

This project focuses on analyzing customer churn in a banking dataset using **Exploratory Data Analysis (EDA)** and data visualization. The aim is to understand customer characteristics, transaction behavior, and other factors that may be associated with customer churn.

The analysis was performed using Python and common data analysis and visualization libraries. Different charts and statistical techniques were used to identify patterns and generate useful insights from the dataset.

##  Objectives

* Understand the structure and characteristics of the bank customer dataset.
* Clean and prepare the data for analysis.
* Identify missing values and handle them appropriately.
* Analyze the distribution of customer churn.
* Study the relationship between customer demographics and churn.
* Analyze banking and transaction-related variables.
* Explore correlations between numerical variables and churn.
* Generate meaningful business insights and recommendations.

##  Dataset

The dataset contains information about **28,382 bank customers** and **22 variables**.

Some of the important columns include:

* `customer_id` – Unique customer identifier
* `vintage` – Customer relationship duration
* `age` – Customer age
* `gender` – Customer gender
* `dependents` – Number of dependents
* `occupation` – Customer occupation
* `city` – Customer city
* `customer_nw_category` – Customer net-worth category
* `branch_code` – Branch identifier
* `current_balance` – Current account balance
* `previous_month_end_balance` – Previous month's ending balance
* `current_month_credit` – Current month's credit amount
* `current_month_debit` – Current month's debit amount
* `churn` – Customer churn status
* `last_transaction` – Date of the customer's last transaction

##  Tools and Technologies

* **Python**
* **Pandas** – Data manipulation and analysis
* **NumPy** – Numerical operations
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical visualization
* **Jupyter Notebook / VS Code** – Development environment

##  Data Cleaning

The dataset was checked for missing values, duplicate records, and data types.

The main cleaning steps included:

* Identifying missing values.
* Filling missing categorical values such as gender, occupation, and city with `"Unknown"`.
* Handling missing values in `dependents` using the median.
* Checking duplicate records.
* Converting and processing transaction date information.
* Creating a `transaction_recency` feature to study how recently customers made transactions.

Missing `last_transaction` values were not artificially replaced with a transaction date because doing so could create misleading information about customer activity.

##  Exploratory Data Analysis

The following areas were analyzed:

1. Customer Churn Distribution
2. Age Distribution
3. Age vs Churn
4. Gender vs Churn
5. Occupation vs Churn
6. Age Group vs Churn
7. Dependents vs Churn
8. Customer Net-Worth Category vs Churn
9. Current Balance vs Churn
10. Current Month Credit vs Churn
11. Current Month Debit vs Churn
12. Vintage vs Churn
13. Transaction Recency vs Churn

Various visualizations such as bar charts, histograms, box plots, and other suitable charts were used to understand the data.

##  Key Findings

* The dataset contains **28,382 customers**.
* There are **5,260 churned customers** and **23,122 non-churned customers**.
* The overall churn rate is approximately **18.53%**.
* Male customers showed a slightly higher churn percentage than female customers in this dataset.
* The **26–35 age group** had the highest churn percentage among the analyzed age groups.
* Age and vintage showed considerable overlap between churned and non-churned customers.
* Transaction recency provided useful information about customer activity.
* Numerical correlations with churn were generally weak, suggesting that churn is not strongly explained by a single numerical variable.

##  Business Insights

The analysis suggests that customer churn may be influenced by a combination of demographic, financial, and behavioral factors rather than one particular variable.

Customers with signs of reduced activity can be monitored and targeted with suitable engagement strategies. Banks can also segment customers based on their characteristics and transaction behavior to improve customer retention.

##  Recommendations

* Identify customers showing reduced transaction activity.
* Develop targeted customer retention campaigns.
* Monitor customer transaction behavior regularly.
* Use customer segmentation to provide more relevant services.
* Analyze multiple customer characteristics together instead of relying on a single variable.
* Build predictive churn models in future work to identify customers who are more likely to leave.

##  Limitations

* The analysis is based on a single dataset.
* Correlation does not imply causation.
* Some variables contain missing values.
* The analysis mainly focuses on exploratory patterns rather than predicting future churn.
* External factors affecting customer decisions were not available in the dataset.

##  Future Scope

This project can be extended by developing a machine learning model to predict customer churn.

Possible future work includes:

* Feature engineering
* Customer segmentation
* Logistic Regression
* Decision Tree
* Random Forest
* XGBoost
* Model evaluation using accuracy, precision, recall, F1-score, and ROC-AUC
* Identifying customers with a high probability of churn

##  Project Structure

```text
Bank_Customer_Churn_Analysis/
│
├── data/
│   └── bank_customer_churn.csv
│
├── notebooks/
│   └── bank_customer_churn_analysis.ipynb
│
├── report/
│   ├── Bank_Customer_Churn_Analysis.docx
│   └── charts/
│
├── screenshots/
│   ├── 01_dataset_preview.png
│   ├── 02_dataset_information.png
│   ├── 03_missing_values.png
│   ├── 04_data_cleaning.png
│   ├── 05_duplicate_check.png
│   ├── 06_churn_analysis.png
│   ├── 07_transaction_recency.png
│   └── 08_correlation_analysis.png
│
└── README.md
```

##  Author

**Aiman**

 Internship Project – 2026

##  Conclusion

This project provided practical experience in data cleaning, exploratory data analysis, visualization, and interpretation using Python. The analysis helped identify patterns in customer churn and demonstrated how data can be used to understand customer behavior and support business decision-making.
