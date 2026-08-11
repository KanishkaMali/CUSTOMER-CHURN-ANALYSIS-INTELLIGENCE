# 🎯 Business Objective

The main objective of this project is to analyze customer churn and identify the customer segments, subscription patterns, and customer-experience signals associated with higher observed churn.

### Key objectives

* Calculate overall customer churn and retention
* Identify high-churn subscription plans
* Compare monthly vs annual contract behavior
* Analyze customer satisfaction and support interactions
* Understand cancellation reasons
* Analyze churn by geography and time
* Quantify revenue and customer-value exposure
* Identify customers requiring retention attention
* Develop actionable business recommendations

---

# 🧩 Business Questions

The analysis answers the following questions:

1. What is the overall churn rate?
2. How many customers have churned?
3. Which subscription plan has the highest observed churn?
4. How does churn differ between monthly and annual contracts?
5. Do churned customers have lower CSAT?
6. Are support escalations associated with churn?
7. What are the major cancellation reasons?
8. Which states show higher observed churn?
9. When is cancellation activity concentrated?
10. What revenue is associated with churned customers?
11. What is the customer value exposure from churn?
12. Which customer segments should be prioritized for retention?

---

# 🗂️ Dataset

The project combines customer, subscription, and support-related information.

### Customer Information

* Customer ID
* Customer Name
* Gender
* Date of Birth
* Country
* State

### Subscription Information

* Subscription Start Date
* Subscription Type
* Plan Type
* Contract Type
* Renewal Date
* Cancellation Date
* Cancellation Reason
* Monthly Charges
* Customer Lifetime Value
* Churn Score

### Customer Support Information

* Complaint Date
* Complaint Count
* Escalations
* CSAT Score
* Support-related information

---

# 🛠️ Tech Stack

## SQL

* PostgreSQL
* SQL Queries
* JOINs
* GROUP BY
* Aggregations
* CASE statements
* Filtering
* Business KPI calculations

## Python

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

## Business Intelligence

* Microsoft Power BI
* DAX
* Data Modeling
* KPI Cards
* Interactive Visualizations
* Slicers
* Dashboard Navigation

## Documentation

* Microsoft PowerPoint
* Microsoft Word
* GitHub

---

# 🔄 Project Workflow

## 1. Data Collection & SQL

The customer data was loaded into a relational database and analyzed using SQL.

SQL was used for:

* Data exploration
* Customer-level analysis
* Aggregation
* Churn calculations
* Revenue analysis
* Segment comparisons
* Business KPI development

---

## 2. Data Cleaning with Python

Python and Pandas were used to prepare the data for analysis.

### Data cleaning activities

* Checked missing values
* Validated data types
* Standardized column names
* Checked duplicate records
* Validated categorical values
* Checked date fields
* Validated churn indicators
* Performed data quality checks

---

## 3. Feature Engineering

Additional analytical features were created to support churn analysis.

### Examples

* Churn Flag
* Customer Tenure
* Churn Status
* Customer Risk Score
* Revenue-related metrics
* Customer value indicators

---

# 📈 Exploratory Data Analysis

Python was used to perform exploratory analysis using:

* GroupBy analysis
* Aggregations
* Pivot tables
* Customer segmentation
* Distribution analysis
* Churn comparisons
* Revenue analysis
* Time-based analysis

### Visualization Libraries

* Matplotlib
* Seaborn

EDA helped identify important patterns before building the Power BI dashboard.

---

# 📊 Power BI Dashboard

The cleaned analytical data was imported into Power BI to build an interactive customer churn dashboard.

### Dashboard capabilities

The dashboard provides analysis of:

* Total Customers
* Churned Customers
* Retained Customers
* Churn Rate
* Retention Rate
* ARPU
* Revenue
* CLTV
* Plan-level churn
* Contract-level churn
* Customer satisfaction
* Support escalations
* Cancellation reasons
* State-level churn
* Churn timing
* Customer risk indicators

---

# 📌 Key KPIs

| KPI                                              | Observed Result |
| ------------------------------------------------ | --------------: |
| Total Customers                                  |              21 |
| Churned Customers                                |               6 |
| Churn Rate                                       |          28.57% |
| Retention Rate                                   |           71.4% |
| Basic Plan Churn                                 |          60.00% |
| Monthly Contract Churn                           |          55.56% |
| Annual Contract Churn                            |           8.33% |
| Average Tenure                                   |      1,451 days |
| ARPU                                             |           ₹18.8 |
| Total Revenue                                    |            ₹395 |
| Revenue Associated with Churned Customers        |             ₹74 |
| Estimated CLTV Associated with Churned Customers |          ₹2,047 |
| Escalation Rate                                  |          19.05% |

> **Note:** These are dataset-level observations based on the current project dataset and should not be interpreted as population-level company metrics.

---

# 🔎 Key Business Insights

## 1️⃣ Overall Churn Rate — 28.57%

6 out of 21 customers have churned.

This results in an observed churn rate of:

**28.57%**

while the observed retention rate is:

**71.4%**

The dataset indicates a customer-retention challenge and provides a basis for identifying higher-risk customer segments.

---

## 2️⃣ Basic Plan Has the Highest Observed Churn

| Plan     | Churn Rate |
| -------- | ---------: |
| Basic    | **60.00%** |
| Standard |     22.22% |
| Premium  |     14.29% |

Basic-plan customers show the highest observed churn rate.

### Recommendation

Investigate:

* Pricing/value perception
* Feature availability
* Content offering
* Service quality
* Competitor positioning

The analysis does not establish that pricing alone caused churn.

---

## 3️⃣ Monthly Contracts Have Much Higher Churn

| Contract Type | Churn Rate |
| ------------- | ---------: |
| Monthly       | **55.56%** |
| Annual        |  **8.33%** |

Monthly-contract customers show a substantially higher observed churn rate than annual-contract customers.

### Recommendation

The business could:

* Encourage annual subscriptions
* Introduce annual-plan incentives
* Provide loyalty benefits
* Target monthly customers with retention campaigns
* Provide personalized renewal offers

This is one of the strongest patterns identified in the analysis.

---

## 4️⃣ Churned Customers Have Lower CSAT

Average CSAT:

| Customer Status | Average CSAT |
| --------------- | -----------: |
| Retained        |          ≈42 |
| Churned         |          ≈34 |

Churned customers show lower average customer satisfaction than retained customers.

### Recommendation

Prioritize customers with:

* Low CSAT
* Recent complaints
* Support escalations
* High churn scores

for proactive customer-success intervention.

---

## 5️⃣ Support Escalations Are an Important Warning Signal

The dashboard reports an escalation rate of approximately:

**19.05%**

Escalation activity appears in the churn-status analysis.

### Recommendation

Create a support escalation follow-up process and proactively engage customers with unresolved issues.

> The analysis indicates an association worth investigating; it does not prove that escalations cause churn.

---

## 6️⃣ Cancellation Reasons Reveal Multiple Churn Drivers

Observed cancellation reasons include:

* Switched to competitor
* Forgot to cancel trial
* Not enough content
* Poor streaming quality
* Too expensive

### Business Interpretation

Customer cancellations appear to involve multiple potential factors:

**Competition + Pricing/Value + Content + Service Quality**

### Recommendation

Create reason-specific retention strategies instead of using a single retention approach for every customer.

---

## 7️⃣ September 2024 Shows Higher Cancellation Activity

The dataset shows the highest observed cancellation activity in:

**September 2024**

### Recommendation

Investigate whether the following changed around this period:

* Pricing
* Product features
* Content
* Technical/service quality
* Promotions
* Competitor activity
* Renewal policies

The dashboard identifies the period for investigation but does not prove the cause.

---

## 8️⃣ Geographic Churn Requires Caution

Karnataka shows the highest observed state-level churn in the current dataset.

However, the dataset contains only 21 customers.

Therefore, state-level percentages can be highly unstable.

### Recommendation

Use geographic results as exploratory signals and validate them using a larger dataset before making regional business decisions.

---

# 💰 Revenue & Customer Value Impact

The analysis identified:

### Total Revenue

**₹395**

### Revenue Associated with Churned Customers

**₹74**

### Estimated CLTV Associated with Churned Customers

**₹2,047**

### Revenue Exposure

Approximately:

**18.7%**

of the analyzed revenue is associated with churned customers based on the project's calculation.

These metrics help demonstrate that churn is not only a customer-retention problem but also a potential revenue and customer-value problem.

---

# 🎯 Customer Risk Prioritization

A customer should not be prioritized based only on churn score.

A stronger retention strategy combines:

```text
Churn Risk
     +
Customer Value
     +
Customer Experience
     ↓
Retention Priority
```

### Important signals

* High churn score
* High CLTV
* Low CSAT
* Recent complaints
* Support escalations
* Monthly contract
* Basic plan

### Recommended Priority

**High-risk + High-value + Poor customer experience**

customers should receive the highest retention priority.

---

# 💡 Business Recommendations

| Priority | Finding                             | Recommended Action                           |
| -------- | ----------------------------------- | -------------------------------------------- |
| 1        | Monthly churn = 55.56%              | Develop annual-plan migration campaigns      |
| 2        | Basic churn = 60%                   | Investigate Basic-plan value proposition     |
| 3        | Churned CSAT is lower               | Proactively engage dissatisfied customers    |
| 4        | Escalations present                 | Improve support escalation resolution        |
| 5        | Competitor switching observed       | Monitor competitor pricing/features          |
| 6        | September cancellation peak         | Investigate events during the period         |
| 7        | Karnataka shows high observed churn | Investigate regional issues with larger data |
| 8        | High-risk customers                 | Prioritize using churn score + CLTV + CSAT   |

---

# 📊 Dashboard Screenshots

## Executive Churn Overview

<img width="386" height="250" alt="image" src="https://github.com/user-attachments/assets/1a4dfa84-1cca-47c6-9677-a4820807b197" />

---

## Customer & Support Intelligence

<img width="540" height="270" alt="image" src="https://github.com/user-attachments/assets/8d27caa5-fbb0-4f1e-b103-7cbca0b481fe" />


---

## Churn Analysis & Segmentation

<img width="383" height="302" alt="image" src="https://github.com/user-attachments/assets/c3731d9e-ca4a-4299-97ce-312e9a7e0402" />


> Replace the image paths above with your actual screenshot filenames.

---

# 📁 Project Structure

```text
Customer-Behavior-Analysis-Using-SQL-Python-Power-BI/
│
├── data/
│   └── customer_churn_data.csv
│
├── sql/
│   ├── data_quality.sql
│   ├── churn_analysis.sql
│   └── business_kpis.sql
│
├── python/
│   └── churn_analysis.ipynb
│
├── powerbi/
│   └── customer_churn_dashboard.pbix
│
├── screenshots/
│   ├── dashboard_1.png
│   ├── dashboard_2.png
│   └── dashboard_3.png
│
├── report/
│   └── Customer_Churn_Analysis_Insight_Report.pdf
│
├── presentation/
│   └── Customer_Churn_Analysis.pptx
│
└── README.md
```

> Update the filenames to match the actual files in your repository.

---

# 🧠 Skills Demonstrated

### Data Analytics

* Data Cleaning
* Data Validation
* Exploratory Data Analysis
* Feature Engineering
* Customer Segmentation
* KPI Development
* Business Analysis

### SQL

* SELECT
* WHERE
* GROUP BY
* ORDER BY
* CASE
* Aggregations
* JOINs
* Customer-level analysis

### Python

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

### Power BI

* Data Modeling
* DAX
* KPI Cards
* Interactive Visualizations
* Slicers
* Dashboard Design
* Business Intelligence

### Business Skills

* Churn Analysis
* Retention Analysis
* Customer Experience Analysis
* Revenue Impact Analysis
* CLTV Analysis
* Risk Prioritization
* Business Recommendations

---

# ⚠️ Project Limitations

This project is based on a relatively small dataset containing 21 customer records.

Therefore:

* Churn percentages are dataset-level observations.
* Small segments can produce extreme percentages.
* Geographic comparisons require a larger sample.
* Observed relationships do not establish causation.
* Churn-risk scoring requires validation on historical outcomes.
* Revenue and CLTV values depend on the project's calculation methodology.

---

# 🚀 Future Improvements

With a larger dataset, this project could be extended with:

### 1. Churn Prediction

Develop a machine-learning model to predict future churn.

### 2. Cohort Analysis

Analyze retention by acquisition month, subscription start period, or customer cohort.

### 3. Customer Lifetime Analysis

Compare CLTV across plans, contracts, and customer segments.

### 4. Automated Dashboard Refresh

Connect Power BI directly to the database for automated reporting.

### 5. Retention Campaign Measurement

Measure whether retention campaigns actually reduce churn.

### 6. Advanced Customer Segmentation

Use clustering techniques to identify behavioral customer segments.

---

# 📌 Final Project Outcome

This project demonstrates a complete end-to-end Data Analyst workflow:

**SQL → Python → Data Cleaning → EDA → Feature Engineering → KPI Development → Power BI → DAX → Business Insights → Recommendations**

The analysis transformed raw customer and subscription data into an interactive churn intelligence solution that identifies higher-risk customer segments, quantifies observed revenue/customer-value exposure, and translates analytical findings into actionable retention strategies.

---

# 👨‍💻 Author

## Kanishka Mali

**Aspiring Data Analyst**

### Technical Skills

`SQL` `Python` `Pandas` `NumPy` `Power BI` `DAX` `Excel` `Data Visualization` `EDA` `Business Analytics`

---

## ⭐ If you found this project useful

Feel free to explore the repository and connect with me for feedback or collaboration.

---



That structure will make it immediately obvious to a recruiter that this is **not just a Power BI dashboard**—it's a complete Data Analyst project.
