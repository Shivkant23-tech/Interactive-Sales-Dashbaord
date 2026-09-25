# 📊 Interactive Dashboard Analysis

## 📌 Project Overview

This project presents an **Interactive Statistical Analysis Dashboard** designed to explore, analyze, and visualize **Customer Churn** and **Sales** datasets.

The dashboard converts statistical analysis into interactive visualizations and business insights. It covers descriptive statistics, probability distributions, correlation analysis, hypothesis testing, confidence intervals, regression analysis, and actionable business recommendations.

The analysis is based on:

* **Customer Churn Dataset** — 500 records
* **Sales Dataset** — 100 records

---

## 🎯 Project Objectives

The main objectives of this project are:

* Analyze customer churn behavior.
* Understand sales performance.
* Explore distributions of numerical variables.
* Identify relationships between variables.
* Perform statistical hypothesis tests.
* Calculate confidence intervals and margins of error.
* Analyze relationships using regression.
* Create interactive charts and dashboards.
* Convert statistical results into business insights.

---

## 📂 Datasets

### Customer Churn Dataset

Key variables include:

* Tenure
* MonthlyCharges
* TotalCharges
* Contract
* Churn

The dataset contains **500 customer records**.

### Sales Dataset

Key variables include:

* Quantity
* Price
* Total_Sales
* Region
* Product Category

The dataset contains **100 sales records**.

---

## 📊 Dashboard Features

### 1. Descriptive Statistics

The dashboard calculates:

* Mean
* Median
* Mode
* Standard deviation
* Variance
* Minimum
* Maximum
* Range
* Skewness
* Kurtosis

For example, the Customer Churn analysis found an average tenure of **36.53** and average MonthlyCharges of **113.64**.

---

### 2. Distribution Analysis

Interactive distribution visualizations include:

* Histograms
* Distribution comparisons
* Q-Q plots
* Normality testing

The analysis uses the **Shapiro-Wilk test** to evaluate whether numerical variables follow a normal distribution. The tested customer churn variables were found to be non-normal.

---

### 3. Correlation Analysis

The dashboard provides correlation analysis using the **Pearson correlation coefficient**.

Correlation values range from:

```text
-1 → Perfect negative correlation
 0 → No linear correlation
+1 → Perfect positive correlation
```

For the Sales dataset:

* Quantity vs Total_Sales: **r = 0.688**
* Price vs Total_Sales: **r = 0.646**
* Quantity vs Price: **r = 0.008**

This shows that Total_Sales has a stronger relationship with Quantity and Price than Quantity and Price have with each other.

---

### 4. Hypothesis Testing

The dashboard presents statistical tests using:

* Two-sample t-tests
* One-way ANOVA
* p-values
* Significance level α = 0.05

#### Customer Churn

MonthlyCharges differed significantly between churned and non-churned customers:

```text
Churned:     $129.77
Non-churned: $111.72
p-value:     0.01008
```

Since p < 0.05, the difference is statistically significant in this dataset.

#### Sales

Average Total_Sales differed between East and West regions:

```text
East: $132,612.58
West: $81,689.31
p-value: 0.04548
```

The result is statistically significant at α = 0.05.

---

### 5. Confidence Intervals

The dashboard calculates:

* 90% confidence intervals
* 95% confidence intervals
* 99% confidence intervals
* Margin of error

The estimated overall customer churn rate is:

```text
Churn Rate: 10.6%
95% CI:     7.9% – 13.3%
```

This provides an estimate of the uncertainty surrounding the sample churn rate.

---

### 6. Regression Analysis

Regression analysis is used to investigate relationships between predictor and outcome variables.

#### Customer Churn

Model:

```text
MonthlyCharges ~ Tenure
```

Results:

```text
R²       = 0.0036
p-value  = 0.182932
```

Tenure explains very little of the variation in MonthlyCharges in this dataset.

#### Sales

Multiple regression:

```text
Total_Sales ~ Quantity + Price
```

Result:

```text
R² = 0.8839
Adjusted R² = 0.8815
```

Together, Quantity and Price explain approximately **88.4% of the variance in Total_Sales** in this dataset.

---

## 📈 Interactive Dashboard Sections

The dashboard can be organized into the following sections:

```text
📊 Dashboard
│
├── 🏠 Overview
│
├── 👥 Customer Churn Analysis
│   ├── KPI Cards
│   ├── Churn Rate
│   ├── Customer Distribution
│   ├── Monthly Charges
│   ├── Tenure Analysis
│   └── Correlation Analysis
│
├── 💰 Sales Analysis
│   ├── Total Sales
│   ├── Regional Sales
│   ├── Product Performance
│   ├── Quantity Analysis
│   └── Price Analysis
│
├── 📈 Statistical Analysis
│   ├── Descriptive Statistics
│   ├── Distribution Analysis
│   ├── Hypothesis Testing
│   ├── Confidence Intervals
│   └── Regression
│
└── 💡 Business Insights
    ├── Customer Retention
    ├── Sales Performance
    ├── Regional Analysis
    └── Recommendations
```

---

## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **SciPy**
* **Matplotlib**
* **Seaborn**
* **Plotly**
* **Streamlit**
* **Excel**
* **Jupyter Notebook**

---

## 🔄 Data Analysis Workflow

```text
Raw Data
   ↓
Data Loading
   ↓
Data Cleaning
   ↓
Exploratory Data Analysis
   ↓
Descriptive Statistics
   ↓
Distribution Analysis
   ↓
Correlation Analysis
   ↓
Hypothesis Testing
   ↓
Confidence Intervals
   ↓
Regression Analysis
   ↓
Interactive Visualizations
   ↓
Business Insights
```

---

## 📁 Project Structure

```text
interactive-dashboard-analysis/
│
├── data/
│   ├── customer_churn.xlsx
│   └── sales_data.xlsx
│
├── dashboard/
│   └── app.py
│
├── analysis/
│   ├── descriptive_analysis.py
│   ├── distribution_analysis.py
│   ├── correlation_analysis.py
│   ├── hypothesis_testing.py
│   ├── confidence_intervals.py
│   └── regression_analysis.py
│
├── notebooks/
│   └── statistical_analysis.ipynb
│
├── reports/
│   └── statistical_analysis_report.pdf
│
├── requirements.txt
└── README.md
```

---

## 🚀 Installation

Clone the repository:

```bash
git clone https://github.com/your-username/interactive-dashboard-analysis.git
```

Move into the project directory:

```bash
cd interactive-dashboard-analysis
```

Install the required libraries:

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Dashboard

If the dashboard is built with Streamlit:

```bash
streamlit run dashboard/app.py
```

The application will open in your browser.

---

## 📌 Key Business Insights

### Customer Churn

* Churned customers have higher average MonthlyCharges than non-churned customers.
* The observed churn rate is **10.6%**.
* Tenure and MonthlyCharges have very weak correlation in this dataset.
* Contract type did not show a statistically significant difference in MonthlyCharges.

### Sales

* Total_Sales is strongly related to Quantity and Price together.
* The East region has higher average Total_Sales than the West region in this dataset.
* Laptop and Phone have the highest average order values among the listed categories.
* Total_Sales is right-skewed, indicating that some large orders have a substantial effect on the average.

---

## 💡 Future Improvements

Possible future improvements include:

* Add real-time data integration.
* Add user authentication.
* Add advanced filtering.
* Add downloadable reports.
* Add automated statistical testing.
* Add machine-learning-based churn prediction.
* Add sales forecasting.
* Add anomaly/outlier detection.
* Deploy the dashboard to a cloud platform.
* Add automated periodic analysis.

The source report specifically suggests building a churn-prediction model using features such as MonthlyCharges, Contract, and PaymentMethod, and periodically rerunning the analysis to monitor churn and regional sales patterns.

---

## 📚 Learning Outcomes

Through this project, the following skills are demonstrated:

* Statistical analysis
* Exploratory Data Analysis (EDA)
* Data visualization
* Probability and distributions
* Hypothesis testing
* p-value interpretation
* Correlation and covariance
* Confidence intervals
* Regression analysis
* Business intelligence
* Dashboard development
* Python data analysis
* Data-driven decision support
