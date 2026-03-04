# 🚀 End-to-End Marketing Analytics Pipeline
**Tech Stack:** `Oracle Data Integrator (ODI)` | `Teradata Vantage` | `Python (Jupyter)` | `CRM & Marketing APIs`

## 📌 Project Overview
This project demonstrates a complete **Enterprise Data Pipeline** that bridges the gap between fragmented marketing efforts and sales revenue. It automates the ingestion, transformation, and modeling of data from various sources (CRM, Ads APIs, Web Events) into a high-performance **Teradata Warehouse**.

The primary goal is to provide a single source of truth for calculating critical business KPIs like **ROAS (Return on Ad Spend)** and **CPL (Cost Per Lead)**.

---

## 🏗️ Pipeline Architecture

### 1. Data Ingestion (Bronze Layer)
* **Tools:** Oracle Data Integrator (ODI)
* **Source Systems:** * **CRM Data:** Lead and Opportunity extracts (`.csv`).
    * **Marketing APIs:** Daily Ad Spend from Google/Meta Ads.
    * **Web Events:** User behavior tracking data.
* **Process:** Using ODI Mappings and Models to load raw files into Teradata landing tables.

### 2. Data Transformation (Silver & Gold Layers)
* **Tools:** Python, TeradataML, Jupyter Notebook
* **Process:** * **Silver Layer:** Cleaning, handling nulls, and standardizing platform names via Python logic.
    * **Gold Layer:** Joining Ad Spend with CRM conversions to create a unified marketing funnel table.
    * **In-Database Processing:** Leveraged `teradataml` to execute heavy transformations directly within the Teradata engine.

---

## 📂 Repository Structure
* **📁 Data Source/**: Sample raw datasets representing CRM and API outputs.
* **📁 Oracle Data Integrator/**: 
    * `Mappings/`: Visual logic for data movement from source to bronze.
    * `Models/`: Data structures defined in ODI.
    * `PROJ_Marketing_Project.xml`: The complete ODI project export for portability.
* **📁 Teradata/**: 
    * `Sql_queries_in_Jupyter_python_interface.ipynb`: The main transformation logic executed via Python.

---

## 🛠️ Key Technical Features
* **Medallion Architecture:** Implemented a structured approach (Bronze → Silver → Gold) to ensure data quality.
* **Complex Data Joining:** Resolved attribution challenges by mapping `UTM_Source` and `Platform` across disparate data silos.
* **Scalability:** Designed with enterprise tools (ODI & Teradata) capable of handling millions of rows.

---

## 📈 Next Steps
* [ ] **Tableau Visualization:** Developing an interactive dashboard to visualize the Marketing Funnel and ROI (Coming Soon).
* [ ] **Automation:** Scheduling the ODI Load Plans for real-time updates.

---
**Contact:**
Mahmoud - [https://www.linkedin.com/in/mahmoud-mamdouh-324125220/]
