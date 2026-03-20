# 🌍 Global Data Jobs Analysis (EDA)

## 📌 Project Overview

This project performs an in-depth **Exploratory Data Analysis (EDA)** on a global dataset of data-related job postings. The goal is to uncover meaningful insights about:

* Salary distributions
  n- Skill-based salary premiums
* Geographic salary differences (India vs USA)
* Remote vs non-remote compensation
* Data cleaning and statistical validation techniques

This project demonstrates strong capabilities in **data wrangling, statistical thinking, and business-oriented analysis**, making it highly relevant for entry-level data analyst roles.

---

## 📂 Project Structure

```
GLOBAL DATA JOBS ANALYSIS/
│
├── data/
│   └── global_jobs_data.xlsx        # Dataset
│
|── power bi/                        # Data Visualization 
|   └── datajobs_visualization.pbit
|   └── visualization.pdf
│   └── job_analysis_images/
|        └── job_postings_flat.csv
|        └── job_postings_flat.csv
|        └── job_postings_flat.csv
|        └── job_postings_flat.csv
|        └── job_postings_flat.csv
|        └── job_postings_flat.csv
|        └── job_postings_flat.csv
|     
├── datajobs_venv/                  # Virtual environment (not tracked)
├── datajobs_analysis.ipynb         # Main analysis notebook
├── .gitignore
├── requirements.txt
├── README.md
├── LICENSE
```

---

## Power BI Dashboard & Visual Insights

Power BI was used as the primary visualization and business intelligence tool in this project. While Python handled statistical validation and data preparation, Power BI enabled interactive exploration, trend analysis, and decision-focused insights.

Below are the key dashboards and insights derived:

🌍 1. Global Job Distribution & Role Comparison

 Insights:

Data Engineer roles dominate hiring volume, followed by Data Analyst and Data Scientist roles

Despite lower volume, Cloud Engineers and Machine Learning Engineers command higher salaries

Senior roles show higher compensation but lower job counts, indicating specialization

 Business Understanding:

The market favors data infrastructure roles (Data Engineering)

High-paying roles are skill-intensive and less saturated

💰 2. Highest Paying Data Roles

📌 Insights:

Senior Data Scientist (~$156K) and Machine Learning Engineer (~$155K) are the top-paying roles

Followed by Senior Data Engineer and Software Engineer roles

Entry-level roles like Data Analyst (~$90K) are significantly lower

📌 Business Understanding:

Compensation strongly correlates with:

Experience (Senior roles)

Technical depth (ML, Engineering)

🌎 3. Salary Comparison Across Top Countries

📌 Insights:

Countries like the USA, UK, and Germany offer higher salaries

India shows lower salary levels, but similar role hierarchy

Senior Data Engineer and Data Scientist roles dominate globally

📌 Business Understanding:

Clear geographic salary disparity

Supports global hiring cost strategies

📈 4. Hiring Trends Over Time (2026)

📌 Insights:

Hiring peaks during July–September

Hiring drops in November–December

Trend consistent across roles

📌 Business Understanding:

Reflects seasonal hiring cycles

End-of-year slowdown due to budget constraints

🧠 5. Skills vs Degree & Work Trends

📌 Insights:

~33% of jobs do not require a degree

Senior roles more likely to mention degrees

~87% jobs allow remote work, yet ~91% are full-time

📌 Business Understanding:

Shift toward skills-first hiring

Remote work is normalized, but job structure remains traditional

🌐 6. Global Job Density Map

📌 Insights:

High job density in:

North America

Europe

India (emerging hub)

Lower presence in developing regions

📌 Business Understanding:

Data jobs cluster in tech-driven economies

Emerging markets show growth potential

🎯 Final Power BI Insights

Data Engineering is the most in-demand role globally

Senior roles command significantly higher salaries

Strong geographic salary inequality exists

Hiring follows seasonal patterns

Industry is shifting toward skills over degrees

Remote work is common, but full-time roles dominate
---

## 🧰 Tech Stack

* **Python**
* **Pandas** – Data manipulation
* **NumPy** – Statistical operations
* **Matplotlib / Seaborn** – Visualization
* **Power BI** - Visualization

---

## 🧹 Data Cleaning & Preparation

Key preprocessing steps performed:

* Converted `job_posted_date` to datetime format
* Converted salary columns to numeric format
* Handled missing values in salary columns
* Removed rows with missing job titles
* Created clean subsets for statistical analysis

---

## 📊 Key Analyses Performed

### 1. Salary Distribution Analysis

* Identified overall salary distribution
* Observed:

  * Mean salary ≈ **$120K**
  * Median salary ≈ **$113K**
  * Maximum salary ≈ **$920K**

 **Insight:**

* The dataset shows a **right-skewed distribution**
* A few extremely high salaries pull the average upward

---

### 2. Outlier Detection using IQR

Used Interquartile Range (IQR) to detect outliers:

* Q1 (25th percentile)
* Q3 (75th percentile)
* IQR = Q3 - Q1

Outliers defined as:

```
Lower Bound = Q1 - 1.5 * IQR
Upper Bound = Q3 + 1.5 * IQR
```

 **Insight:**

* Significant high-end salary outliers exist
* Median is a more reliable measure than mean in skewed distributions

---

### 3. Salary Band Segmentation (Quantile-Based)

Used `pd.qcut()` to divide salaries into 4 equal groups:

* Low
* Mid
* High
* Very High

 **Insight:**

* Each band contains ~25% of data
* Demonstrates balanced segmentation using quantiles

---

 **Insight:**

* Observed salary differences are **statistically significant**
* Not due to random chance

---

### 4. Variability & Distribution Analysis

Analyzed:

* Standard deviation
* Skewness
* Spread of salaries

 **Insight:**

* High standard deviation indicates wide salary variation
* Outliers significantly impact distribution

---

## Key Business Insights

* Salary distributions are **right-skewed** with high-end outliers
* Entry-level roles tend to have **compressed salary bands**
* Senior roles show **higher variability in compensation**
* Geographic location significantly impacts compensation

---

## What This Project Demonstrates

* Strong **data cleaning and wrangling skills**
* Ability to apply **statistical reasoning in real datasets**
* Understanding of **data distributions and outliers**
* Capability to extract **business insights from raw data**
* Experience with **real-world messy datasets**

---

## Final Note

This project is part of my journey to becoming a highly skilled data analyst. It focuses not just on coding, but on **thinking like an analyst — questioning data, validating assumptions, and extracting real-world insights.**

---

## License

This project is licensed under the terms of the LICENSE file included in this repository.

---