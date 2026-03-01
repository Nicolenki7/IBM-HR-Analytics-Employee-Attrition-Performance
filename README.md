# 👔 IBM HR Analytics — Employee Attrition & Performance

**HR Analytics | Logistic Regression | Feature Importance | Business Storytelling**

[![Python](https://img.shields.io/badge/Python-3776AB?logo=python)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikit-learn)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/Pandas-150458?logo=pandas)](https://pandas.pydata.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 📋 Overview

Predictive model for employee attrition with robust feature engineering and coefficient-based driver extraction. Identifies key factors driving employee turnover to enable targeted retention interventions.

This project demonstrates end-to-end HR analytics from data exploration through model interpretation with business storytelling.

---

## 💼 Business Impact

- **Retention Strategy**: Identify at-risk employees before they leave
- **Driver Analysis**: Understand root causes of attrition (coefficients)
- **Cost Reduction**: Lower recruitment and training costs through retention
- **HR Intelligence**: Data-driven workforce planning

---

## 🛠️ Technical Stack

| Category | Technologies |
| :--- | :--- |
| **Data Processing** | Python, Pandas, NumPy |
| **Feature Engineering** | Custom transformations, encoding |
| **Machine Learning** | scikit-learn (Logistic Regression) |
| **Visualization** | Matplotlib, Seaborn |
| **Analysis** | Jupyter Notebooks |

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                  HR ATTRITION ANALYTICS                      │
├─────────────────────────────────────────────────────────────┤
│                                                              │
│  DATA EXPLORATION                                           │
│  └─→ IBM HR Analytics dataset                               │
│      - Demographics, job roles, satisfaction, performance   │
│                                                              │
│  FEATURE ENGINEERING                                        │
│  └─→ Robust transformations:                                │
│      - Categorical encoding (One-Hot, Label)                │
│      - Numerical scaling                                    │
│      - Interaction features                                 │
│                                                              │
│  MODELING (Logistic Regression)                             │
│  └─→ Attrition prediction, coefficient extraction           │
│                                                              │
│  INTERPRETATION                                             │
│  └─→ Feature importance, business storytelling              │
│                                                              │
└─────────────────────────────────────────────────────────────┘
```

---

## 🚀 Key Features

### Feature Engineering
- **Categorical Encoding**: One-hot encoding for job roles, departments
- **Numerical Scaling**: StandardScaler for continuous variables
- **Interaction Features**: Combined metrics (e.g., satisfaction × performance)

### Logistic Regression Model
- **Algorithm**: Logistic Regression with L2 regularization
- **Output**: Attrition probability (0-1)
- **Interpretability**: Coefficient-based feature importance

### Driver Analysis
- **Coefficient Extraction**: Identify positive/negative attrition drivers
- **Odds Ratios**: Quantify impact magnitude
- **Business Storytelling**: Translate technical results to HR actions

---

## 📊 Results & Metrics

| Metric | Value |
| :--- | :--- |
| **Model Type** | Logistic Regression (L2 regularization) |
| **Key Drivers** | Overtime, job satisfaction, years at company |
| **Feature Count** | 30+ engineered features |
| **Interpretability** | Coefficient-based analysis |

---

## 📁 Project Structure

```
IBM-HR-Analytics-Employee-Attrition-Performance/
├── data/                              # Raw and processed data
├── notebooks/                         # Analysis notebooks
│   ├── 01_exploratory_analysis.ipynb
│   ├── 02_feature_engineering.ipynb
│   └── 03_model_training.ipynb
├── src/                               # Python scripts
├── models/                            # Trained model files
├── outputs/                           # Reports, visualizations
└── README.md                          # Project documentation
```

---

## 🔧 Setup & Installation

```bash
# Clone the repository
git clone https://github.com/Nicolenki7/IBM-HR-Analytics-Employee-Attrition-Performance.git
cd IBM-HR-Analytics-Employee-Attrition-Performance

# Install dependencies
pip install -r requirements.txt

# Run exploratory analysis
jupyter notebook notebooks/01_exploratory_analysis.ipynb

# Execute feature engineering
jupyter notebook notebooks/02_feature_engineering.ipynb

# Train model and extract drivers
jupyter notebook notebooks/03_model_training.ipynb
```

---

## 📈 Usage

### Key Attrition Drivers (Coefficient Analysis)

| Factor | Impact | Interpretation |
| :--- | :--- | :--- |
| **Overtime** | High Positive | Employees working overtime 2-3× more likely to leave |
| **Job Satisfaction** | High Negative | Low satisfaction strongly correlates with attrition |
| **Years at Company** | Negative | Longer tenure reduces attrition risk |
| **Monthly Income** | Negative | Higher compensation reduces turnover |
| **Distance from Home** | Positive | Longer commute increases attrition likelihood |

### Business Recommendations
1. **Reduce Overtime**: Review workload distribution
2. **Improve Satisfaction**: Engagement programs, career development
3. **Retention Bonuses**: Target high-risk employees
4. **Flexible Work**: Remote options for long-commute employees

---

## 🎯 Key Learnings

- **Logistic Regression** provides interpretable coefficients for HR stakeholders
- **Feature engineering** improves model performance and insights
- **Coefficient analysis** translates directly to business actions
- **Business storytelling** is critical for HR analytics adoption

---

## 🔮 Future Enhancements

- [ ] Advanced models (Random Forest, XGBoost) with SHAP analysis
- [ ] Survival analysis for time-to-attrition prediction
- [ ] Employee segmentation (clustering)
- [ ] Recommendation engine for retention interventions
- [ ] Integration with HRIS systems for real-time scoring

---

## 🔗 Links

| Resource | URL |
| :--- | :--- |
| **Repository** | https://github.com/Nicolenki7/IBM-HR-Analytics-Employee-Attrition-Performance |
| **Dataset** | [IBM HR Analytics on Kaggle](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset) |

---

## 📝 Resumen en Español

Modelo predictivo de attrition de empleados con feature engineering robusto y extracción de drivers basada en coeficientes.

Los factores principales que impulsan el abandono son: horas extras (overtime), satisfacción laboral, y años en la compañía. El análisis de coeficientes de Regresión Logística permite traducir resultados técnicos a acciones de RRHH accionables.

---

## 📄 License

MIT License — Feel free to fork, modify, and use for personal or commercial projects.

---

## 👤 Author

**Nicolás Zalazar** | Senior Data Engineer & Microsoft Fabric Specialist

- GitHub: [@Nicolenki7](https://github.com/Nicolenki7)
- LinkedIn: [nicolas-zalazar-63340923a](https://www.linkedin.com/in/nicolas-zalazar-63340923a)
- Portfolio: [nicolenki7.github.io/Portfolio](https://nicolenki7.github.io/Portfolio/)
- Email: zalazarn046@gmail.com

---

*Last Updated: March 2026*
