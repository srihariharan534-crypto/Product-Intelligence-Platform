# 🚀 Product Intelligence Platform

## 📌 Overview

The **Product Intelligence Platform** is an end-to-end Data Analytics and Business Intelligence solution designed to analyze customer behavior, product performance, subscription trends, and revenue growth.

The platform transforms raw business data into actionable insights through a fully automated ETL pipeline, SQL data warehouse, advanced analytics modules, and interactive dashboards.

It enables organizations to:

* Improve customer retention
* Identify churn risk
* Increase Customer Lifetime Value (CLV)
* Track revenue growth
* Monitor product performance
* Support data-driven business decisions

---

## 🎯 Business Objectives

* Analyze customer engagement and subscription behavior
* Identify churn patterns and retention opportunities
* Calculate Customer Lifetime Value (CLV)
* Measure Monthly and Annual Recurring Revenue
* Segment customers using RFM Analysis
* Provide executive-level business intelligence dashboards

---

## 🏗️ Solution Architecture

```text
Raw Data Sources
(CSV • Logs • Databases)
          │
          ▼
┌────────────────────┐
│    ETL Pipeline    │
│ Extract • Transform│
│       Load         │
└────────────────────┘
          │
          ▼
┌────────────────────┐
│ SQL Data Warehouse │
│ Star Schema Model  │
└────────────────────┘
          │
          ▼
┌────────────────────┐
│ Analytics Engine   │
│ CLV • Churn • RFM  │
│ Cohort Analysis    │
└────────────────────┘
          │
          ▼
┌────────────────────┐
│ Visualization & BI │
│ Streamlit Dashboard│
│ Power BI Reports   │
└────────────────────┘
```

---

## ✨ Key Features

### 🔄 Automated ETL Pipeline

* Data extraction from multiple sources
* Data cleansing and transformation
* Automated loading into warehouse tables

### 📊 Customer Analytics

* Customer Segmentation (RFM)
* Churn Analysis
* Customer Lifetime Value (CLV)
* Retention Tracking

### 📈 Revenue Analytics

* Monthly Recurring Revenue (MRR)
* Annual Recurring Revenue (ARR)
* Average Revenue Per User (ARPU)
* Revenue Growth Analysis

### 📉 Cohort Analysis

* Monthly Cohort Retention
* User Lifecycle Tracking
* Retention Heatmaps

### 📋 Business Intelligence

* Interactive Streamlit Dashboard
* Power BI Reporting
* Executive PDF Reports

---

## 🛠️ Technology Stack

| Category        | Technologies                |
| --------------- | --------------------------- |
| Programming     | Python                      |
| Database        | MySQL, SQLite               |
| Data Processing | Pandas, NumPy               |
| Analytics       | Scikit-Learn                |
| Visualization   | Streamlit, Plotly, Power BI |
| Reporting       | ReportLab                   |
| Version Control | Git, GitHub                 |

---

## 📂 Project Structure

```text
Product-Intelligence-Platform
│
├── analytics/
├── dashboard/
├── data/
├── docs/
├── etl/
├── notebooks/
├── powerbi/
├── reports/
├── sql/
│
├── requirements.txt
├── LICENSE
└── README.md
```

---

## 📊 KPIs Tracked

* Monthly Recurring Revenue (MRR)
* Annual Recurring Revenue (ARR)
* Customer Lifetime Value (CLV)
* Customer Churn Rate
* Retention Rate
* Average Revenue Per User (ARPU)
* Revenue Growth Rate
* RFM Customer Segments

---

## 🚀 Getting Started

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run ETL Pipeline

```bash
python etl/etl_pipeline.py
```

### Launch Dashboard

```bash
streamlit run dashboard/streamlit_app.py
```

### Generate Executive Report

```bash
python reports/generate_report.py
```

---

## 📈 Business Impact

✔ Improved visibility into customer behavior

✔ Early identification of churn risks

✔ Better customer retention strategies

✔ Revenue optimization through CLV insights

✔ Executive-ready reporting and dashboards

---



