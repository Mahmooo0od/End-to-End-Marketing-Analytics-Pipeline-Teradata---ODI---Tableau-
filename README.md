# 🚀 End-to-End Marketing Analytics Pipeline
**Tech Stack:** `ODI` | `Teradata` | `SQL` | `Python (Jupyter)` | `CRM & APIs`

## 📌 Project Overview
This project demonstrates an enterprise-grade data pipeline. It orchestrates data from **CRM** and **Marketing APIs**, moves it via **Oracle Data Integrator (ODI)**, and performs advanced modeling using **SQL** and **Python** inside **Teradata Vantage**.

---

## 🏗️ Pipeline Architecture & Documentation

### 1. Data Ingestion (ODI)
I used **ODI** to build a robust ingestion layer. Below are the visual mappings and models that represent the data flow from source to the Bronze layer in Teradata.

#### **ODI Mapping Preview:**
![ODI Mapping](./Oracle%20Data%20Integrator/Mappings/Mapping.png)

#### **Detailed Bronze Mappings:**
| Ads Spend | CRM Leads | Web Events |
|---|---|---|
| ![Ads](./Oracle%20Data%20Integrator/Mappings/MAP_BRZ_ADS_SPEND.png) | ![Leads](./Oracle%20Data%20Integrator/Mappings/MAP_BRZ_CRM_CRM_LEADS.png) | ![Web](./Oracle%20Data%20Integrator/Mappings/MAP_BRZ_WEB_EVENTS.png) |

#### **ODI Models Structure:**
![Models](./Oracle%20Data%20Integrator/Models/Models.png)
*Includes: Teradata Target Model, CRM Model, and Flat Files definitions.*

---

### 2. Data Transformation (SQL & Python)
The transformation logic is documented in a Jupyter Notebook. I combined the power of **SQL** for table structures and **teradataml (Python)** for data cleaning and joining the Final Gold Layer.

#### **In-Database Processing:**
> **View Full Script:** [Jupyter Notebook](./Teradata/Sql_queries_in_Jupyter_python_interface.ipynb)

---

## 📂 Repository Structure
* **📁 Data Source/**: Raw CSV samples (`ads_spend_daily.csv`, `crm_leads.csv`, etc.).
* **📁 Oracle Data Integrator/**: 
    * `Mappings/`: Visual ETL flow screenshots.
    * `Models/`: Data structure definitions.
    * `PROJ_Marketing_Project.xml`: The complete exported ODI project.
* **📁 Teradata/**: Python/SQL transformation scripts via Jupyter.

---

## 🛠️ Key Technical Features
* **SQL & Python Hybrid:** Using SQL for DDL and Python for complex DML.
* **Medallion Architecture:** Implementing Bronze, Silver, and Gold layers for data quality.
* **Enterprise Standards:** Full use of ODI for professional ETL orchestration.

---

## 📈 Next Steps
* [ ] **Tableau Visualization:** (Work in Progress) Building the ROI & Attribution Dashboard.

---
**Contact:**
Mahmoud - [https://www.linkedin.com/in/mahmoud-mamdouh-324125220/]
