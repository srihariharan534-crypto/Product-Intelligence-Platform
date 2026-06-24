# Product Intelligence Platform

A production-grade, portfolio-ready Data Analytics platform that processes customer subscriptions, transactional logs, and products data to compute critical SaaS KPIs (MRR, ARR, Churn, Cohort Retention, and RFM Segmentation).

This project features a fully modelled MySQL Star Schema warehouse, an automated python-based ETL pipeline, advanced analytic scoring engines, a programmatic business report builder, and an interactive Streamlit visual dashboard.

---

## 🛠️ Tech Stack & Architecture

* **Language**: Python 3.10+
* **Data Processing**: Pandas, NumPy
* **Analytics Engine**: Scikit-Learn (segmentation options), RFM scoring, cohort retention matrices
* **Database**: MySQL / SQLite (Star Schema layout)
* **Visualization Layer**: Streamlit, Plotly, Power BI
* **Report Generation**: ReportLab (programmatic PDF compiler)

---

## 📂 Folder Structure

```text
Product-Intelligence-Platform/
├── data/
│   ├── raw/                      # Generated CSVs (Customers, Products, Transactions)
│   └── processed/                # Normalized Dim/Fact Tables, Churn, CLV, RFM CSVs
├── sql/
│   ├── schema.sql                # Database initialization script
│   ├── tables.sql                # Star schema table definitions (dim/fact)
│   ├── views.sql                 # SQL views for streamlined reporting
│   └── kpi_queries.sql           # SQL calculations for MRR, Churn, and ARPU
├── etl/
│   ├── extract.py                # Synthetic raw dataset generator (100,000+ records)
│   ├── transform.py              # Dimension modeling, date key expansions
│   ├── load.py                   # Data loader supporting SQLite/MySQL engines
│   └── etl_pipeline.py           # Main pipeline orchestrator
├── analytics/
│   ├── customer_segmentation.py  # RFM segment classifier
│   ├── churn_analysis.py         # Churn rate analysis and attributes mapping
│   ├── clv_analysis.py           # SaaS Predictive & historical CLV calculator
│   ├── cohort_analysis.py        # Monthly signup cohort retention engine
│   └── revenue_analysis.py       # MRR, ARR, and MoM growth calculations
├── dashboard/
│   ├── streamlit_app.py          # Multi-tab Streamlit dashboard app
│   └── assets/                   # Static dashboard logo and materials
├── powerbi/
│   ├── README_PowerBI.md         # DAX formulas, relationship model guide
│   └── Product_Intelligence_Dashboard_Mockup.png # Dashboard visualization mockup
├── notebooks/
│   ├── exploratory_analysis.ipynb # Jupyter notebook for EDA
│   └── business_analysis.ipynb    # Jupyter notebook for segment and cohort analyses
├── docs/
│   ├── architecture_diagram.png  # Platform design layout
│   ├── data_dictionary.md        # Dimensional schema data definitions
│   └── project_documentation.md  # Analytics details and business methodologies
├── reports/
│   └── business_report.pdf       # Programmatically compiled PDF report
├── requirements.txt              # Project package requirements
├── LICENSE                       # MIT License
└── README.md                     # Main documentation page
```

---

## 🚀 Getting Started

### 1. Installation
Clone the repository and install the dependencies:
```bash
pip install -r requirements.txt
```

### 2. Run the ETL & Analytics Pipeline
Execute the main orchestrator script to generate raw data (120,000+ records), transform them into dimensional tables, populate the SQL database, and run all downstream analytics:
```bash
python etl/etl_pipeline.py --customers 15000 --transactions 160000
```

### 3. Launch the Interactive Dashboard
Run the Streamlit app to explore metrics, filters, segments, and heatmaps:
```bash
streamlit run dashboard/streamlit_app.py
```

### 4. Generate Business PDF Report
Recompile the PDF business report containing the latest metrics:
```bash
python reports/generate_report.py
```

---

## 📊 Analytics Summary

* **Customer Segments**: Users are classified into 9 RFM segments (e.g., Champions, Loyal Customers, At Risk, Lost) to tailor retention strategies.
* **Monthly Cohort Retention**: Displays customer persistence over time since their signup period, highlighting operational churn risk points.
* **Revenue Run-Rates**: Uses deferred revenue amortization to spread annual deals across 12 calendar months, presenting highly accurate MRR, ARR, and ARPU metrics.
