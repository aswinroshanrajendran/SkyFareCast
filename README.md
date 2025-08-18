# ✈️ SkyFareCast – Flight Price Prediction System

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Built%20with-Streamlit-orange?logo=streamlit)
![FastAPI](https://img.shields.io/badge/Backend-FastAPI-lightgrey)
![Airflow](https://img.shields.io/badge/Workflow-Airflow-blueviolet)
![Grafana](https://img.shields.io/badge/Monitoring-Grafana-red)
![License](https://img.shields.io/badge/License-MIT-green)

SkyFareCast is a **flight price prediction system** that predicts flight ticket prices, automates scheduled predictions, and provides a monitoring dashboard for model performance and data quality. It combines **user interactivity**, **API endpoints**, **scheduled jobs**, and **visual analytics** in one end-to-end solution.

> 🚀 Built with 💡 curiosity, ✈️ passion for travel, and 🧠 applied machine learning!  

---

## 🌟 Table of Contents

- [Project Highlights](#project-highlights)  
- [Demo Screenshots](#demo-screenshots)  
- [Tech Stack](#tech-stack)  
- [How It Works](#how-it-works)  
- [Project Structure](#project-structure)  
- [Getting Started](#getting-started)  
- [CSV Data](#csv-data)  
- [Conclusion](#conclusion)  

---

## 🌟 Project Highlights

- On-demand flight price predictions through **Streamlit UI**
- **FastAPI backend** to expose ML model and store results in PostgreSQL
- Scheduled predictions with **Airflow DAGs**
- Data validation & preprocessing with **Python**
- Monitoring dashboard using **Grafana**  
  - Pie chart for model performance (accuracy)  
  - Bar chart for high-alert inputs  
- End-to-end pipeline for **data ingestion, validation, prediction, and monitoring**

---

## 📸 Demo Screenshots

| Streamlit App | FastAPI Predictions | Airflow DAGs |
|---------------|------------------|--------------|
| ![Streamlit](images/streamlit_app.png) | ![FastAPI](images/fastapi_prediction.png) | ![Airflow](images/airflow_dags.png) |

| Grafana – Pie Chart | Grafana – Bar Chart |
|--------------------|-------------------|
| ![Pie Chart](images/grafana_pie.png) | ![Bar Chart](images/grafana_bar.png) |

---

## 🛠 Tech Stack

- **Language**: Python 3.10+  
- **Libraries**: 
  - `pandas`, `numpy`, `requests`, `scikit-learn`, `SQLAlchemy`  
- **Web Framework**: Streamlit, FastAPI  
- **Workflow Orchestration**: Apache Airflow  
- **Monitoring & Visualization**: Grafana  
- **Database**: PostgreSQL  
- **IDE**: VS Code  
- **Version Control**: Git + GitHub  

---

## 🧠 How It Works

1. **User Interface (Streamlit)**  
   - Users provide flight details and get real-time predictions.  
   - Historical predictions are displayed with input features.  

2. **ML Model API (FastAPI)**  
   - Exposes `/predict` endpoint for model predictions.  
   - Saves results to the database with features and timestamp.  

3. **Database (PostgreSQL + SQLAlchemy)**  
   - Stores all prediction records.  
   - Enables historical analysis for monitoring model performance.  

4. **Scheduled Prediction Pipeline (Airflow)**  
   - Ingests new data and triggers predictions at defined intervals.  
   - Logs all scheduled runs for auditing and debugging.  

5. **Data Validation & Preprocessing**  
   - Ingested raw data is checked for missing or invalid values.  
   - Cleaned and transformed data is stored as “good data” for predictions.  

6. **Monitoring Dashboard (Grafana)**  
   - **Pie Chart**: Shows model accuracy (`Correct`, `Incorrect`, `Skipped`).  
   - **Bar Chart**: Highlights input features triggering high alerts.  
   - Enables visual tracking of model performance and data quality over time.  

---

## 📂 Project Structure

