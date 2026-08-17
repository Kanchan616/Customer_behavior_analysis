# Customer_behavior_analysis
Data Analytics Project showcasing customer  behavior analysis using python, sql and power BI.
# Data Analytics Project

## Overview

This project demonstrates an end-to-end **data analytics workflow**, from loading and exploring raw data to generating business insights and presenting the results through interactive dashboards and reports.

The project covers:

* Data loading and exploration using Python
* Exploratory Data Analysis (EDA)
* Data cleaning and preprocessing
* SQL-based data analysis
* Interactive Power BI dashboard development
* Analytical report preparation
* Presentation creation using Gamma

---

## Dataset

The project uses a structured dataset containing business-related records for analysis.

The dataset is first loaded into Python, where its structure, data types, missing values, duplicates, and potential data-quality issues are examined before further analysis.

**Dataset format:** CSV / Excel
**Main analysis areas:** Customer, sales, product, category, and other relevant business attributes.

---

## Tools & Technologies

| Tool                                | Purpose                                   |
| ----------------------------------- | ----------------------------------------- |
| **Python**                          | Data loading, cleaning, and EDA           |
| **Pandas**                          | Data manipulation and analysis            |
| **NumPy**                           | Numerical operations                      |
| **Matplotlib / Seaborn**            | Data visualization                        |
| **PostgreSQL / MySQL / SQL Server** | SQL analysis and business queries         |
| **Power BI**                        | Dashboard and data visualization          |
| **Gamma**                           | Presentation development                  |
| **Excel**                           | Data inspection and supporting analysis   |
| **Git & GitHub**                    | Version control and project documentation |

---

## Project Workflow

```text
Raw Dataset
     ↓
Python Data Loading
     ↓
Data Exploration & EDA
     ↓
Data Cleaning & Preprocessing
     ↓
SQL Database
     ↓
SQL Analysis & Business Queries
     ↓
Power BI Dashboard
     ↓
Business Insights & Report
     ↓
Gamma Presentation
```

---

## Steps

### 1. Load the Dataset

The dataset is imported into Python using Pandas.

Key tasks include:

* Loading CSV/Excel files
* Inspecting rows and columns
* Checking data types
* Identifying missing values
* Checking duplicate records
* Understanding the dataset structure

### 2. Exploratory Data Analysis

EDA is performed to understand patterns, trends, and relationships within the data.

Analysis includes:

* Descriptive statistics
* Distribution analysis
* Category-wise analysis
* Trend analysis
* Outlier detection
* Correlation analysis
* Visual exploration

### 3. Data Cleaning

Data-quality issues identified during EDA are addressed.

Typical cleaning activities include:

* Handling missing values
* Removing duplicates
* Correcting data types
* Standardizing categorical values
* Handling invalid records
* Treating outliers where appropriate
* Creating calculated/derived columns

The cleaned dataset is then prepared for SQL and Power BI analysis.

### 4. SQL Analysis

The cleaned data is loaded into a relational database such as **PostgreSQL, MySQL, or SQL Server**.

SQL is used to answer business questions and generate analytical insights.

Queries may include:

* Aggregations using `SUM()`, `AVG()`, and `COUNT()`
* `GROUP BY` analysis
* Filtering with `WHERE` and `HAVING`
* Table joins
* Subqueries
* Common Table Expressions (CTEs)
* Window functions
* Ranking and top-N analysis
* Trend analysis

Example business questions:

```sql
-- Top 5 categories by total sales

SELECT
    category,
    SUM(amount) AS total_sales
FROM sales
GROUP BY category
ORDER BY total_sales DESC
LIMIT 5;
```

> SQL syntax may be adjusted depending on whether PostgreSQL, MySQL, or SQL Server is being used.

### 5. Power BI Dashboard

The cleaned and analyzed data is imported into Power BI to create an interactive dashboard.

The dashboard focuses on key business metrics such as:

* Total Sales
* Total Customers
* Total Orders
* Average Order Value
* Top Products
* Top Categories
* Sales by Region/Location
* Trends over time

Interactive features may include:

* Slicers
* Filters
* Drill-downs
* KPI cards
* Charts
* Tables
* Tooltips

---

## Dashboard

The Power BI dashboard provides an interactive view of the major business KPIs and trends identified during the analysis.

### Dashboard Highlights

* **KPI Overview** – High-level performance metrics
* **Sales Analysis** – Revenue and sales trends
* **Product Analysis** – Best and worst-performing products
* **Category Analysis** – Performance across categories
* **Customer Analysis** – Customer purchasing behavior
* **Geographical Analysis** – Regional performance

> Add screenshots of the final Power BI dashboard here.

```text
![Power BI Dashboard](images/dashboard.png)
```

---

## Results & Key Insights

The analysis is used to identify meaningful business insights rather than simply presenting descriptive statistics.

Key findings may include:

* Highest-performing products and categories
* Lowest-performing areas requiring attention
* Customer purchasing patterns
* Sales trends over time
* Regional performance differences
* Opportunities for improving sales and customer engagement
* Business areas that may require further investigation

The final insights are documented in the project report and presented through the Gamma presentation.

---

## Project Report

A detailed report is prepared to document:

1. Business problem
2. Dataset description
3. Data-cleaning process
4. EDA findings
5. SQL analysis
6. Power BI dashboard
7. Key insights
8. Business recommendations
9. Conclusion

---

## Presentation

A professional presentation is created using **Gamma** to communicate the project's findings to a non-technical audience.

The presentation summarizes:

* Business problem
* Approach and methodology
* Key KPIs
* Major findings
* Dashboard insights
* Business recommendations
* Conclusion

---

## How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/your-repository.git
cd your-repository
```

### 2. Install Python Dependencies

Create a virtual environment if required:

```bash
python -m venv venv
```

Activate it:

**Windows:**

```bash
venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

### 3. Run the Python Analysis

Open the Jupyter Notebook:

```bash
jupyter notebook
```

Run the EDA and data-cleaning notebooks in the recommended order.

### 4. Set Up the Database

Create a database in **PostgreSQL, MySQL, or SQL Server** and import the cleaned dataset.

Update the database connection details according to your environment.

### 5. Run SQL Queries

Open the SQL scripts located in the `sql/` directory and execute them using your preferred database client.

### 6. Open the Power BI Dashboard

Open the `.pbix` file using **Power BI Desktop**.

If necessary, update the data source/database connection and refresh the dataset.

---

## Repository Structure

```text
data-analytics-project/
│
├── data/
│   ├── raw/
│   └── cleaned/
│
├── notebooks/
│   ├── 01_data_loading.ipynb
│   ├── 02_eda.ipynb
│   └── 03_data_cleaning.ipynb
│
├── sql/
│   ├── analysis_queries.sql
│   └── business_questions.sql
│
├── powerbi/
│   └── dashboard.pbix
│
├── report/
│   └── data_analysis_report.pdf
│
├── presentation/
│   └── project_presentation.pdf
│
├── images/
│   └── dashboard.png
│
├── requirements.txt
└── README.md
```

---

## Conclusion

This project demonstrates an end-to-end approach to **data analysis and business intelligence**, combining Python, SQL, and Power BI to transform raw data into actionable insights.

It showcases practical skills in:

**Data Cleaning → EDA → SQL → Data Visualization → Dashboard Development → Business Reporting → Data Storytelling**

The project is designed to demonstrate both **technical data-analysis skills and the ability to communicate business insights effectively**.
