# Customer-Churn-Analysis
End-to-end Customer Churn Analysis using Python. Includes data cleaning, EDA, KPI analysis, customer segmentation, and visualizations to identify key churn drivers, high-risk customers, and actionable insights for improving customer retention.
Customer Churn Analysis — Complete Python Data Analytics Project

# 📌 Project Overview

Customer churn is a major business challenge for subscription-based companies. When customers stop using a company's products or services, the company loses recurring revenue and may need to spend additional resources acquiring new customers.

This project analyzes customer data to identify the major factors associated with customer churn. The analysis follows a complete data analytics workflow, including data import, data understanding, data cleaning, feature engineering, exploratory data analysis (EDA), KPI analysis, visualization, customer segmentation, business insights, and recommendations.

The dataset contains customer demographic information, contract details, internet services, payment methods, tenure, monthly charges, total charges, support tickets, late payments, and churn status.

### Dataset Size:

Raw Dataset: 2,515 rows and 15 columns
Final Dataset: 2,500 rows and 20 columns after cleaning and feature engineering

The project aims to help a business understand which customer groups are more likely to churn and identify potential opportunities for improving customer retention.

# 🎯 Objectives

The main objectives of this project are:

•Calculate the overall customer churn rate.
•Identify the total number of customers and churned customers.
•Analyze churn by contract type.
•Identify regions with higher churn rates.
•Analyze the relationship between customer tenure and churn.
•Examine churn patterns across payment methods.
•Analyze churn by internet service type.
•Compare monthly charges between churned and retained customers.
•Analyze whether support tickets are associated with churn.
•Examine the relationship between late payments and churn.
•Segment customers based on their overall value.
•Identify high-value customers who have churned.
•Generate business insights and provide data-driven retention recommendations.

# 📂 Project Structure
customer-churn-analysis-python/
│
├── customer_churn_data.csv
│
├── Python Customer Churn Analysis Project.ipynb
│
├── README.md
│
└── requirements.txt
Files Description

•customer_churn_data.csv
Contains the raw customer churn dataset used for the analysis.

•Python Customer Churn Analysis Project.ipynb
Contains the complete Python data analysis workflow, including data cleaning, feature engineering, EDA, KPI analysis, visualizations, business insights, and recommendations.
*Complete Python Notebook Script:*
**[Customer_Churn_Analysis_Project](Customer_Churn_Analysis_Project)**
# README.md
Provides an overview of the project, objectives, technologies, analysis process, key findings, and instructions for running the project.

requirements.txt
Contains the Python libraries required to run the project.

# 🛠️ Technologies Used

The following technologies and libraries were used in this project:

### Programming Language
Python
Data Analysis
Pandas
NumPy
Data Visualization
Matplotlib
Seaborn
Development Environment
Jupyter Notebook
Key Data Analysis Techniques
Data Cleaning
Missing Value Treatment
Duplicate Removal
Data Type Conversion
Text Standardization
Feature Engineering
Exploratory Data Analysis
GroupBy and Aggregation
Customer Segmentation
KPI Analysis
Correlation Analysis
Business Insight Generation

# 🔄 Project Workflow

The project follows the complete data analyst workflow:

Import Libraries
       ↓
Import CSV Dataset
       ↓
Understand Dataset
       ↓
Data Cleaning
       ↓
Feature Engineering
       ↓
Data Quality Check
       ↓
KPI Analysis
       ↓
Exploratory Data Analysis
       ↓
Customer Segmentation
       ↓
Visualization
       ↓
Business Insights
       ↓
Recommendations

# 🧹 Data Cleaning

Several data cleaning steps were performed to improve data quality.

1. Duplicate Check

Duplicate records were identified and removed from the dataset.

Raw records: 2,515
Final records after duplicate removal: 2,500
Duplicate records removed: 15
2. Missing Value Analysis

Missing values were checked across all columns.

The following treatment was applied:

Missing values in numerical columns such as monthly_charges and support_tickets were filled using the median.
Missing values in payment_method were filled using the mode.
3. Text Cleaning

Text columns were cleaned by:

Removing unnecessary spaces.
Standardizing text formatting.
Cleaning categorical values.
Standardizing region and payment method labels.
4. Date Conversion

The signup_date column was converted into a proper datetime format.

5. Data Validation

The dataset was checked for potential data quality issues, including:

Age below 18.
Negative monthly charges.
Negative total charges.
Negative customer tenure.
⚙️ Feature Engineering

Additional features were created to support deeper analysis.

Estimated Annual Value
estimated_annual_value = monthly_charges * 12

This estimates the annual revenue value of each customer.

Average Monthly Revenue

This feature calculates customer revenue relative to their tenure.

avg_monthly_revenue = total_charges / tenure_months
Age Group

Customers were segmented into the following age groups:

18–25
26–35
36–45
46–55
56–65
65+
Tenure Group

Customers were categorized based on how long they have been associated with the company:

0–6 Months
7–12 Months
13–24 Months
25–48 Months
49–72 Months
Customer Value Segment

Customers were divided into three value categories based on total charges:

Low Value
Medium Value
High Value

# 🔍 Exploratory Data Analysis (EDA)

The project performs exploratory data analysis to understand customer behavior and identify churn patterns.

The following analyses were performed:

1. Churn Distribution

The distribution of customers who churned versus customers who remained was analyzed.

2. Churn by Contract Type

Customer churn rates were compared across different contract types to identify which contracts have higher customer loss.

3. Churn by Region

Churn rates were analyzed across geographical regions.

4. Churn by Payment Method

Different payment methods were compared to identify whether billing and payment behavior may be associated with churn.

5. Churn by Internet Service

Customer churn was analyzed across different internet service categories.

6. Tenure Analysis

Customer tenure groups were compared to understand how customer retention changes over time.

7. Monthly Charges vs Churn

Monthly charges of churned and non-churned customers were compared using visualization.

8. Support Tickets vs Churn

The average number of support tickets was analyzed for churned and retained customers.

9. Late Payments vs Churn

Late payment behavior was compared between churned and retained customers.

10. Customer Value Analysis

Customers were segmented into low, medium, and high-value groups to analyze revenue and churn.

11. High-Value Customers at Risk

High-value customers who churned were identified as an important business and revenue risk.

12. Correlation Analysis

A correlation heatmap was created to analyze relationships between numerical variables, including:

Age
Tenure
Monthly Charges
Total Charges
Support Tickets
Late Payments
📊 Key KPIs

The following key performance indicators were calculated:

KPI	Result
Total Customers	2,500
Churned Customers	538
Overall Churn Rate	21.52%
Total Customer Revenue	₹7,221,821
Average Monthly Charge	₹79.13

# 💡 Key Insights
1. Overall Customer Churn Rate

The overall customer churn rate is 21.52%, with 538 out of 2,500 customers identified as churned.

This indicates that customer retention is an important area for business improvement.

2. Contract Type Has a Strong Relationship with Churn

Month-to-month customers show the highest churn rate at approximately 31.94% among the main standardized contract categories.

Longer-term contracts have substantially lower churn:

Two Year: approximately 12.26%
One Year: approximately 9.66%

This suggests that customers with longer commitments are more likely to remain with the company.

3. Early-Tenure Customers Are More Likely to Churn

The highest churn rate occurs among customers with short tenure.

Tenure Group	Churn Rate
0–6 Months	35.90%
7–12 Months	30.80%
13–24 Months	30.00%
25–48 Months	20.28%
49–72 Months	12.60%

This shows that customer retention improves significantly as tenure increases.

4. South Region Has the Highest Churn

The South region has the highest churn rate at approximately 23.48%.

The churn rates across regions are relatively close, but regional differences may help management prioritize retention campaigns.

5. Fiber Optic Customers Have Higher Churn

Customers using Fiber Optic service show the highest churn rate at approximately 25.87%.

This may indicate an opportunity to investigate service quality, pricing, customer expectations, or support experience.

6. Customers Who Churn Pay Higher Monthly Charges

The average monthly charge for churned customers is approximately ₹88.31, compared with approximately ₹76.62 for customers who did not churn.

This suggests that higher pricing may be associated with increased churn risk.

7. Churned Customers Generate More Support Tickets

Churned customers have an average of approximately 2.35 support tickets, compared with approximately 2.04 for retained customers.

This suggests that customer service issues and repeated support interactions may be associated with churn.

8. Late Payments Are Higher Among Churned Customers

Churned customers have more average late payments than retained customers.

Churned customers: approximately 1.12
Retained customers: approximately 0.96

This could indicate billing difficulties or customer engagement issues before churn occurs.

9. Electronic Check Has the Highest Payment-Method Churn

Electronic Check customers show the highest churn rate at approximately 22.25%.

Although the differences between payment methods are relatively small, payment experience and billing friction should be investigated further.

10. High-Value Customer Churn Represents Revenue Risk

The analysis identified 142 high-value customers who churned.

Even though the high-value segment has a lower churn rate than the low-value segment, losing high-value customers can have a significant impact on revenue.

These customers should be considered a priority for retention programs.

# 📈 Visualizations Created

The project includes the following visualizations:

•Customer Churn Distribution
•Churn Rate by Contract Type
•Churn Rate by Region
•Churn Rate by Payment Method
•Churn Rate by Internet Service
•Churn Rate by Customer Tenure
•Monthly Charges by Churn Status
•Average Support Tickets by Churn Status
•Average Late Payments by Churn Status
•Revenue by Customer Value Segment
•Correlation Matrix Heatmap

# 📌 Business Recommendations

Based on the analysis, the following recommendations can help reduce customer churn:

1. Focus on Month-to-Month Customers

Provide targeted retention offers, discounts, loyalty benefits, or incentives to encourage customers to move to one-year or two-year contracts.

2. Improve Early Customer Experience

Customers in their first 6–12 months have the highest churn rates.

The company should improve onboarding, provide proactive communication, and identify customer problems early.

3. Investigate Fiber Optic Customer Experience

Fiber Optic customers have the highest churn rate. The business should investigate:

Service quality
Pricing
Customer complaints
Network performance
Support experience
4. Monitor High-Value Customers

Create a priority retention strategy for high-value customers who show potential churn signals.

Possible signals include:

Multiple support tickets
Late payments
High monthly charges
Short customer tenure
5. Improve Customer Support

Customers with more support tickets show higher churn.

The company should identify recurring customer problems and improve support resolution time and service quality.

6. Review Pricing Strategy

Since churned customers have higher average monthly charges, the company should investigate whether pricing, perceived value, or competitive alternatives contribute to customer loss.

7. Improve Payment Experience

Analyze Electronic Check and other payment processes for possible billing friction, payment failures, or customer experience problems.

# ▶️ How to Run the Project

Step 1: Clone the Repository
git clone <your-github-repository-url>
Step 2: Navigate to the Project Folder
cd customer-churn-analysis-python
Step 3: Install Required Libraries
pip install pandas numpy matplotlib seaborn jupyter
Step 4: Start Jupyter Notebook
jupyter notebook
Step 5: Open the Notebook

Open:

Python Customer Churn Analysis Project.ipynb
Step 6: Update the Dataset Path

Make sure the CSV file path in the notebook points to your dataset.

For example:

df = pd.read_csv("customer_churn_data.csv")
Step 7: Run All Cells

Run the notebook from top to bottom to perform:

Data Import
→ Data Cleaning
→ Feature Engineering
→ KPI Analysis
→ EDA
→ Visualization
→ Business Insights
→ Recommendations

# 📦 Requirements

Create a requirements.txt file with:

pandas
numpy
matplotlib
seaborn
jupyter

Install all dependencies using:

pip install -r requirements.txt

# 🚀 Future Improvements

This project can be further improved in the following ways:

1. Build a Machine Learning Churn Prediction Model

Use machine learning algorithms to predict customers who are likely to churn.

Possible models include:

Logistic Regression
Random Forest
Decision Tree
XGBoost
2. Create an Interactive Dashboard

Build an interactive dashboard using:

Power BI
Tableau
Streamlit

The dashboard could allow management to monitor churn KPIs and customer segments in real time.

3. Add Customer Churn Prediction Scores

Assign each customer a churn risk score, such as:

Low Risk
Medium Risk
High Risk
4. Perform Advanced Statistical Analysis

Conduct additional statistical testing to determine whether observed differences between customer groups are statistically significant.

5. Analyze Customer Behavior Over Time

Use signup dates and additional time-based data to analyze churn trends by:

Month
Quarter
Year
Customer cohort
6. Develop an Automated Retention Strategy

Create a rule-based or machine-learning-based system that automatically identifies customers requiring retention actions.

7. Improve Data Quality Validation

Add more automated checks for:

Inconsistent category labels
Invalid values
Outliers
Unexpected missing values

# 🧠 Skills Demonstrated

This project demonstrates the following Data Analyst skills:

Python
Pandas
NumPy
Data Cleaning
Data Validation
Missing Value Handling
Duplicate Removal
Feature Engineering
Exploratory Data Analysis
Data Aggregation
GroupBy Analysis
Customer Segmentation
KPI Development
Business Analysis
Data Visualization
Matplotlib
Seaborn
Correlation Analysis
Business Insight Generation
Data-Driven Recommendations

# 📬 Conclusion

This project demonstrates an end-to-end customer churn analysis workflow using Python. The analysis identifies important churn patterns related to contract type, customer tenure, monthly charges, internet service, support activity, payment behavior, and customer value.

The findings can help businesses identify at-risk customer groups and develop targeted retention strategies to reduce churn and protect revenue.
