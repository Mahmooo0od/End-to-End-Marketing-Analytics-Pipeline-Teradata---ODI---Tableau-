# 🚀 End-to-End Marketing Analytics Pipeline
**Tech Stack:** `ODI` | `Teradata` | `SQL` | `Python (Jupyter)` | `CRM & APIs`

## 📌 Project Overview
This project demonstrates an enterprise-grade data pipeline. It orchestrates data from **CRM** and **Marketing APIs**, moves it via **Oracle Data Integrator (ODI)**, and performs advanced modeling using **SQL** and **Python** inside **Teradata Vantage**.

The goal is to automate **ROAS** and **CPL** calculations by unifying disparate data silos.

---

## 🏗️ Pipeline Architecture & Documentation

### 1. Data Ingestion (ODI)
Using **Oracle Data Integrator**, I built the ingestion layer to move raw data into the Teradata Bronze layer.
* **Mappings:** Visual logic for data flow.
* **Models:** Relational structures for Ads and CRM data.

> **View ODI Work:** > [Check Mappings Screenshots](./Oracle%20Data%20Integrator/Mappings/)  
> [Check Models Screenshots](./Oracle%20Data%20Integrator/Models/)



---

### 2. Data Transformation (SQL & Python)
The transformation logic follows the **Medallion Architecture**. I used **SQL** for structural queries and **Python (teradataml)** for complex data cleansing.

* **SQL Core:** Defining table schemas, primary keys, and relations in Teradata.
* **Python Logic:** Handling string normalization, Null treatments, and final Gold table joins.

> **View Scripts:** > [Jupyter Notebook (SQL/Python)](./Teradata/Sql_queries_in_Jupyter_python_interface.ipynb)



---

## 📂 Repository Structure
* **📁 Data Source/**: Raw CSV samples (CRM & API mocks).
* **📁 Oracle Data Integrator/**: 
    * `Mappings/`: Screenshots of ETL flows.
    * `Models/`: Screenshots of data definitions.
    * `PROJ_Marketing_Project.xml`: Full ODI project export.
* **📁 Teradata/**: 
    * `Sql_queries_in_Jupyter_python_interface.ipynb`: Transformation logic.

---

## 🛠️ Key Technical Features
* **Multi-Language Pipeline:** Seamless integration between **SQL** for data definition and **Python** for logic.
* **Enterprise Ingestion:** Using **ODI** for robust, scalable data movement.
* **Data Integrity:** Ensuring consistency between "Anonymous" Ad clicks and "Identified" CRM Leads.

---

## 📈 Next Steps
* [ ] **Tableau Visualization:** (Work in Progress) Building the ROI & Attribution Dashboard.
* [ ] **Load Plan Automation:** Scheduling the end-to-end flow.

---
**Contact:**
Mahmoud - [LinkedIn Profile Link]
