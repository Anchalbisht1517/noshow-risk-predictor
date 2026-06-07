# 🏥 CarePredict – Medical Appointment No-Show Prediction System

[![Streamlit App](https://img.shields.io/badge/Live%20Demo-Streamlit-red?logo=streamlit)](https://noshow-risk-predictor-i.streamlit.app/)
[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)]()
[![XGBoost](https://img.shields.io/badge/Model-XGBoost-green.svg)]()
[![SHAP](https://img.shields.io/badge/Explainability-SHAP-orange.svg)]()
[![Streamlit](https://img.shields.io/badge/Frontend-Streamlit-red.svg)]()
[![License](https://img.shields.io/badge/License-Educational-lightgrey.svg)]()

## 🌐 Live Demo

🚀 **Try the Application Here**

👉 **https://noshow-risk-predictor-i.streamlit.app/**

The live application provides real-time patient no-show risk prediction, explainable AI insights, healthcare analytics, and operational decision support tools for hospitals and clinics.

---

# 📌 Project Overview

CarePredict is an AI-powered healthcare analytics platform designed to predict medical appointment no-shows before they occur. The system leverages Machine Learning, Explainable AI (SHAP), and an interactive Streamlit dashboard to help healthcare institutions proactively identify high-risk patients, reduce operational losses, improve scheduling efficiency, and enhance patient care.

The platform transforms raw appointment scheduling data into actionable insights through a complete end-to-end machine learning pipeline.

---

# 🎯 Problem Statement

Healthcare institutions worldwide lose millions of dollars annually due to missed appointments. When patients fail to attend scheduled appointments:

- Physician time remains unused
- Medical resources are wasted
- Revenue leakage increases
- Patient waiting lists grow
- Care continuity is disrupted

Traditional reminder systems treat all patients equally and fail to identify patients who are genuinely at risk of missing appointments.

CarePredict solves this challenge by predicting the probability of no-show events and recommending targeted intervention strategies before the appointment occurs.

---

# 🚀 Key Features

## 🤖 Machine Learning Engine

- Binary Classification Prediction
- No-Show Risk Assessment
- Multi-Model Comparison
- Automated Data Processing
- Probability-Based Risk Scoring

### Implemented Models

- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost (Primary Production Model)

---

## 🧠 Explainable AI

CarePredict integrates SHAP (SHapley Additive Explanations) to provide transparent predictions.

### Global Explainability

- Feature Importance Ranking
- SHAP Summary Plot
- SHAP Bar Chart
- Feature Contribution Analysis

### Local Explainability

- Individual Patient Explanations
- Waterfall Charts
- Force Plots
- Risk Driver Identification

---

## 📊 Interactive Dashboard

### Dashboard Overview

Executive-level KPIs and hospital performance metrics.

### Daily Briefing

Operational insights for hospital administrators.

### Patient Risk Assessment

Single patient prediction interface.

### Batch Upload Prediction

CSV-based bulk prediction processing.

### Risk Queue

High-risk patient prioritization.

### EDA Explorer

Interactive exploratory data analysis.

### SHAP Insights

Model explainability interface.

### Model Health

Performance monitoring dashboard.

### Reports

Exportable reports and analytics.

---

# 📂 Dataset Information

## Dataset Source

Medical Appointment No-Shows Dataset (Kaggle)

### Dataset Statistics

| Metric | Value |
|----------|----------|
| Total Records | 110,527 |
| Raw Features | 14 |
| Attendance Rate | 79.8% |
| No-Show Rate | 20.2% |
| Class Imbalance | 4:1 |
| Country | Brazil |
| City | Vitória, Espírito Santo |

---

# 🔍 Features Used

## Original Features

- Gender
- Age
- Neighbourhood
- Scholarship
- Hypertension
- Diabetes
- Alcoholism
- Handicap
- SMS Received
- Scheduled Day
- Appointment Day

---

## Engineered Features

### 1. days_waiting

Number of days between appointment scheduling and appointment date.

### 2. age_group

Patient age categories:

- Child
- Teenager
- Adult
- Senior
- Elderly

### 3. appointment_weekday

Day of the week when appointment occurs.

### 4. wait_bucket

Appointment waiting time categories:

- 0–7 Days
- 8–14 Days
- 15–30 Days
- 31–60 Days
- 60+ Days

### 5. previous_no_shows

Historical count of previous missed appointments.

---

# 🏗️ System Architecture

```text
                    ┌────────────────────┐
                    │   Raw CSV Dataset  │
                    └──────────┬─────────┘
                               │
                               ▼
                    ┌────────────────────┐
                    │ Data Ingestion     │
                    └──────────┬─────────┘
                               │
                               ▼
                    ┌────────────────────┐
                    │ Data Validation    │
                    └──────────┬─────────┘
                               │
                               ▼
                    ┌────────────────────┐
                    │ Data Cleaning      │
                    └──────────┬─────────┘
                               │
                               ▼
                    ┌────────────────────┐
                    │ Feature Engineering│
                    └──────────┬─────────┘
                               │
                               ▼
                    ┌────────────────────┐
                    │ Data Transformation│
                    └──────────┬─────────┘
                               │
                               ▼
                    ┌────────────────────┐
                    │ Model Training     │
                    └──────────┬─────────┘
                               │
                               ▼
                    ┌────────────────────┐
                    │ Model Evaluation   │
                    └──────────┬─────────┘
                               │
                               ▼
                    ┌────────────────────┐
                    │ SHAP Explainability│
                    └──────────┬─────────┘
                               │
                               ▼
                    ┌────────────────────┐
                    │ Streamlit Dashboard│
                    └────────────────────┘
```

---

# ⚙️ Project Workflow

## Phase 1 – Data Ingestion

- CSV Loading
- Datetime Parsing
- Metadata Collection

## Phase 2 – Data Validation

- Schema Validation
- Data Quality Checks
- Validation Reporting

## Phase 3 – Data Cleaning

- Invalid Record Removal
- Outlier Detection
- Data Standardization

## Phase 4 – Feature Engineering

- Derived Feature Creation
- Leakage Prevention
- Behavioral Feature Generation

## Phase 5 – Data Transformation

- Train-Test Split
- Encoding
- Scaling
- SMOTE Resampling

## Phase 6 – Model Training

- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost

## Phase 7 – Model Evaluation

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC

## Phase 8 – SHAP Explainability

- Global Feature Analysis
- Patient-Level Explanations

## Phase 9 – EDA Visualization

- Business Intelligence Charts
- Data Insights

## Phase 10 – Application Development

- Streamlit Integration
- Dashboard Deployment

---

# 📈 Model Evaluation Metrics

Models are evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC Score
- Confusion Matrix
- Classification Report

---

# 🛠️ Technology Stack

## Programming Language

- Python

## Machine Learning

- Scikit-Learn
- XGBoost
- Imbalanced-Learn

## Explainable AI

- SHAP

## Data Processing

- Pandas
- NumPy

## Data Visualization

- Plotly
- Matplotlib
- Seaborn

## Dashboard

- Streamlit

## Configuration Management

- YAML

## Version Control

- Git
- GitHub

---

# 📁 Project Structure

```text
CarePredict/
│
├── .streamlit/
│
├── config/
│   ├── config.yaml
│   ├── params.yaml
│   └── schema.yaml
│
├── data/
│   ├── raw/
│   └── processed/
│
├── artifacts/
│
├── models/
│
├── outputs/
│   ├── plots/
│   └── reports/
│
├── notebooks/
│
├── src/
│   ├── components/
│   ├── pipeline/
│   ├── entity/
│   ├── exception/
│   └── utils/
│
├── app.py
├── main.py
├── requirements.txt
├── setup.py
└── README.md
```

---

# 📦 Installation

## Clone Repository

```bash
git clone https://github.com/yourusername/CarePredict.git
```

```bash
cd CarePredict
```

---

## Create Virtual Environment

```bash
python -m venv venv
```

---

## Activate Environment

### Windows

```bash
venv\Scripts\activate
```

### Linux / Mac

```bash
source venv/bin/activate
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

# ▶️ Running the Project

## Train Models

```bash
python main.py
```

---

## Launch Streamlit Dashboard

```bash
streamlit run app.py
```

---

# 📊 Business Impact

CarePredict enables healthcare organizations to:

✅ Reduce appointment no-shows

✅ Improve hospital resource utilization

✅ Increase operational efficiency

✅ Improve patient engagement

✅ Enable proactive interventions

✅ Improve healthcare accessibility

✅ Support data-driven decision making

---

# 🔮 Future Enhancements

## Version 2

- Automated Retraining
- Better Risk Recommendations
- Enhanced Reporting System
- Notification Engine

## Version 3

- FastAPI Backend
- PostgreSQL Database
- Kubernetes Deployment
- Electronic Health Record Integration
- Multi-Hospital Deployment
- Real-Time Prediction Service
- Drift Detection Framework

---

# 👨‍💻 Contributors

### Project Lead

- Machine Learning Development
- Model Evaluation

### Data Engineering

- Data Collection
- Data Analysis
- Feature Engineering

### Deployment & DevOps

- Streamlit Deployment
- CI/CD Setup

---

# 📜 License

This project is developed for:

- Academic Learning
- Research Purposes
- Portfolio Demonstration
- Educational Use

---

# ⭐ Acknowledgements

- Kaggle Medical Appointment No-Shows Dataset
- Scikit-Learn Community
- XGBoost Team
- SHAP Framework
- Streamlit Community
- Open Source Contributors

---

## 🌟 Live Application

🚀 **Access CarePredict Here**

### https://noshow-risk-predictor-i.streamlit.app/

If you find this project useful, consider giving it a ⭐ on GitHub.
