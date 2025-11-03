# 📊 IBM HR ANALYTICS: PREDICTIVE EMPLOYEE ATTRITION (CHURN) ANALYSIS

## 🎯 Project Objective
This Data Science and Business Intelligence project aims to **identify and quantify the primary risk factors driving voluntary employee attrition (Churn)** within a sample of the IBM HR Analytics dataset.

The analysis uses a predictive model (Logistic Regression) to extract key "Churn Drivers" and presents the results in a concise, interactive dashboard, fully ready for strategic Human Resources decision-making.

## 🔗 LIVE DASHBOARD LINK
You can access the live, interactive Looker Studio dashboard here:

[IBM HR Churn Dashboard](https://lookerstudio.google.com/s/vwyerWvTjZk)

## 🛠️ Methodology and Technologies

The workflow was executed in three distinct phases:

### 1. Data Preparation and Modeling (Python)
* **Language:** Python 3.x
* **Key Libraries:**
    * `pandas`: Data cleaning, missing value imputation, and initial Feature Engineering.
    * `scikit-learn`: Implementation of the **Logistic Regression** model for driver analysis and coefficient extraction.
    * `sqlite3`: Used for in-memory SQL Feature Engineering to create strategic employee segments.

### 2. Feature Engineering (FE)
Strategic categorical variables were created in the Python script to enhance the descriptive analysis:
* `Attrition_Numeric`: Binary target variable (1: Attrition, 0: No Attrition).
* `Seniority_Category`: Categories based on `TotalWorkingYears` (Entry, Mid, Senior, Veteran Level).
* `Monthly_Income_Level`: Income ranges for segmentation (Low, Medium, High Income).

### 3. Visualization and Business Intelligence
* **BI Tool:** **Looker Studio** (Google Data Studio)
* **Final Design:** **Canva** (Used for the polished executive layout).

---

## 📈 DASHBOARD STRUCTURE

The final dashboard is divided into two key pages, designed to answer critical business questions:

### Page 1: Executive Summary & Predictive Drivers
* **Purpose:** Answers the **"Why?"** by quantifying influence.
* **Key Elements:**
    * **KPIs:** Total Attrition Rate (16.12%), Total Employees, Average Years at Company.
    * **Bar Chart:** TOP 10 Churn Drivers (Coeficientes).
    * **Scatter Plot:** Distributes drivers by **Impact Direction** (Positive/Negative) vs. **Magnitude**.

### Page 2: Descriptive Analysis and Segmentation
* **Purpose:** Answers the **"Who and Where is the risk?"** by segmenting the population.
* **Key Elements:**
    * **Attrition by Tenure:** Churn rate segmented by `YearsAtCompany` (showing the critical risk peak in the 0-2 year range).
    * **FE Segments:** Churn rates by `Monthly_Income_Level` and `Seniority_Category`.
    * **Risk Distribution:** Analysis of churn across Department, Job Satisfaction levels, and the critical impact of `OverTime`.

---

## 💡 EXECUTIVE KEY FINDINGS

The analysis highlights three critical and immediately actionable risk areas:

| Key Finding | Strategic Focus |
| :--- | :--- |
| **1. Extreme Workload is Primary.** **Overtime** is the single highest predictor of attrition across the entire dataset. | **Load Management:** Immediately review Overtime policies and prioritize headcount investment in high-friction roles (e.g., Lab Technicians). |
| **2. High Early-Career Churn.** Attrition peaks within the **first 5 years** of service and the `Entry_Level` segment. | **Retention Programs:** Fortify early-career *onboarding* and mentorship efforts for employees with under 3 years of tenure. |
| **3. Financial & Satisfaction Gaps.** Risk is highest in the **Low Income** segment and among employees reporting minimum **Job Satisfaction** (Score 1). | **Targeted Review:** Conduct competitive salary reviews for the 'Low Income' segment and implement immediate intervention plans for employees reporting minimum satisfaction. |

---

## 📂 Repository Files

| File | Description |
| :--- | :--- |
| `HR.csv` | The original source dataset used for the analysis. |
| `hr_data_fe_ready.csv` | The final clean output from the Python script, ready for BI consumption. |
| `hr_churn_drivers.csv` | The output from the Logistic Regression model, containing features and their coefficients. |
| `IBM_HR_Analytics (1).pdf` | The final two-page executive dashboard report. |
| `[python script file]` | The complete Python code for data cleaning, FE, and model training. |

## 🚀 How to Reproduce the Analysis

1.  **Clone the Repository:** `git clone [Your Repository URL]`
2.  **Install Dependencies:** Install the required Python libraries (`pandas`, `scikit-learn`, `numpy`).
3.  **Run the Python Script:** Execute the script to generate the final `hr_data_fe_ready.csv` and `hr_churn_drivers.csv` files.
4.  **Access Dashboard:** View the final product via the **Live Dashboard Link** above.
