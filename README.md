# Intelligent Supplier Risk Prediction & Analytics

An intelligent, machine-learning-based system that analyses supplier financial data, operational performance, and supplier-related news to identify potential risks and support better supply-chain decisions.

## 🚀 Live Application

**Streamlit App:** https://sheetal-092-supplier-risk-prediction-app-bwg8kj.streamlit.app/

## 📌 Project Overview

Supplier-related problems such as financial instability, delivery delays, quality issues, increasing costs, and negative business news can affect supply-chain operations.

Traditional supplier risk assessment often depends on historical records and manual analysis. This project addresses these challenges by combining financial, operational, and news-related information with machine learning techniques.

The system provides supplier risk prediction, supplier segmentation, anomaly detection, news sentiment analysis, and early-warning indicators through an interactive Streamlit dashboard.

## 🎯 Objectives

- Predict supplier risk using financial and operational data.
- Analyse supplier-related news using FinBERT sentiment analysis.
- Study changes in news sentiment over time using LSTM.
- Classify suppliers into Low, Medium, and High Risk categories.
- Group suppliers with similar characteristics using K-Means.
- Detect unusual supplier behaviour using Isolation Forest.
- Explain model predictions using SHAP.
- Monitor supplier risk trends and generate early-warning alerts.
- Provide an interactive dashboard for supplier risk analysis.

## ✨ Key Features

### 1. Dataset Analysis
- Upload supplier datasets in CSV, XLSX, and XLS formats.
- Load sample financial and operational datasets.
- Validate and preprocess uploaded supplier records.
- View supplier information and risk-related metrics.

### 2. Supplier Risk Prediction
- Uses XGBoost for structured financial and operational risk prediction.
- Uses Random Forest as a comparison model.
- Identifies potential high-risk suppliers.
- Displays supplier risk scores and risk categories.

### 3. News Sentiment Analysis
- Uses FinBERT to analyse supplier-related financial and business news.
- Identifies positive, neutral, and negative sentiment.
- Uses sentiment information as an additional supplier-risk signal.

### 4. Temporal Sentiment Analysis
- Uses LSTM to examine sequences of supplier news sentiment.
- Identifies changes in sentiment over time.
- Supports early identification of potentially increasing risks.

### 5. Supplier Segmentation
- Uses K-Means clustering to group suppliers with similar financial and operational characteristics.
- Helps compare supplier performance patterns.

### 6. Anomaly Detection
- Uses Isolation Forest to identify unusual supplier records.
- Highlights abnormal operational or financial patterns for further investigation.

### 7. Explainable AI
- Uses SHAP (SHapley Additive exPlanations) to explain the contribution of individual features to structured-data predictions.
- Helps users understand the factors influencing supplier risk.

### 8. Live Monitoring
- Provides a simulated Live Data Mode.
- Demonstrates changes in supplier risk indicators over time.
- Displays monitoring trends and anomaly alerts.

**Note:** Live Data Mode uses simulated records for demonstration. It is not a connection to real-time external supplier databases.

## 🧠 Technologies Used

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Dashboard | Streamlit |
| Data Processing | Pandas, NumPy, PySpark |
| Machine Learning | XGBoost, Random Forest |
| NLP | FinBERT |
| Deep Learning | LSTM |
| Clustering | K-Means |
| Anomaly Detection | Isolation Forest |
| Explainable AI | SHAP |
| Data Visualization | Plotly |
| Cloud Storage | Microsoft Azure |
| Business Intelligence | Power BI |

## 🏗️ System Workflow

```text
Supplier Financial Data
Supplier Operational Data
Supplier-Related News
          |
          v
    Data Collection
          |
          v
 Data Preprocessing
   PySpark / Pandas
          |
          v
   Feature Engineering
          |
          v
  +-------------------------+
  |  Financial and          |
  |  Operational Prediction |
  |  XGBoost / Random Forest|
  +-------------------------+
          |
          v
  +-------------------------+
  | News Sentiment Analysis |
  |       FinBERT           |
  +-------------------------+
          |
          v
  +-------------------------+
  | Temporal Analysis       |
  |       LSTM              |
  +-------------------------+
          |
          v
     Risk Integration
          |
          v
  +-------------------------+
  | Supplier Segmentation   |
  | K-Means                 |
  +-------------------------+
          |
          v
  +-------------------------+
  | Anomaly Detection       |
  | Isolation Forest        |
  +-------------------------+
          |
          v
     SHAP Explanations
          |
          v
    Streamlit Dashboard
          |
          v
 Risk Analysis, Alerts,
 Trends and Monitoring
```

## 📊 Dashboard Modules

The application provides the following navigation sections:

- **Overview:** Overall supplier-risk summary.
- **Supplier Analytics:** Supplier performance and analytical insights.
- **Risk Prediction:** Supplier-level risk prediction.
- **Anomaly & Alerts:** Unusual records and risk alerts.
- **Live Monitoring:** Simulated supplier monitoring over time.

## ⚙️ Installation and Execution

### Prerequisites

- Python 3.9 or later
- pip package manager
- Git

### 1. Clone the Repository

```bash
git clone https://github.com/sheetal-092/KLH-CSE-2026_2027-TEAM_5-INTELLIGENT_SUPPLIER_RISK_PREDICTION.git
```

### 2. Navigate to the Project Folder

```bash
cd KLH-CSE-2026_2027-TEAM_5-INTELLIGENT_SUPPLIER_RISK_PREDICTION
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

### 5. Run the Application

```bash
streamlit run app.py
```

Open the local URL displayed in the terminal to access the dashboard.

## 📁 Project Structure

```text
Intelligent-Supplier-Risk-Prediction/
│
├── app.py
├── requirements.txt
├── README.md
│
├── data/
│   ├── financial_sample.csv
│   └── operational_sample.csv
│
├── models/
│   ├── xgboost_model
│   ├── random_forest_model
│   └── other_model_files
│
├── notebooks/
│   └── data_preprocessing_and_model_training.ipynb
│
└── images/
    └── dashboard_screenshot.png
```

*The structure above is a suggested layout. Update the filenames and folders to match the actual repository.*

## 📂 Dataset Information

The project supports financial, operational, and supplier-related news information.

The financial sample described in the project contains 250 suppliers and a 90-day disruption label. The application also provides an operational sample containing simulated delivery and performance metrics.

Users can upload their own supplier datasets in supported formats.

**Important:** Sample or simulated data is intended for development and demonstration. It should not be treated as verified real-world supplier information.

## 👩‍💻 Project Team

**Gullapalli Sheetal**  
Email: sheetalgullapalli92@gmail.com

**Jangari Sakshitha**  
Email: sakshijangari@gmail.com

**Gullapalli Nikitha Chowdary**  
Email: nikithachowdarygullapalli@gmail.com

## 👩‍🏫 Project Guide

**Dr. N. Shirisha**  
Associate Professor  
Department of Computer Science and Engineering

Koneru Lakshmaiah Education Foundation  
Hyderabad, Telangana, India

## 🔮 Future Enhancements

- Integration with real-time supplier data sources and APIs.
- Improved supplier news collection and monitoring.
- More advanced risk prediction and model evaluation.
- Cloud-based deployment and scalable data processing.
- Enhanced early-warning notifications.
- Improved dashboard reporting and analytics.

## 📜 License

This project was developed for academic and educational purposes as part of the B.Tech Computer Science and Engineering capstone project.
