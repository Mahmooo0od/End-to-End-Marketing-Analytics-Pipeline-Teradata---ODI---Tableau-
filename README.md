# 🚀 End-to-End Marketing Analytics Pipeline
**Tech Stack:** `ODI` | `Teradata` | `SQL` | `Python (Jupyter)` | `CRM & APIs`

## 📌 Project Overview
This project demonstrates an enterprise-grade data pipeline. It orchestrates data from **CRM** and **Marketing APIs**, moves it via **Oracle Data Integrator (ODI)**, and performs advanced modeling using **SQL** and **Python** inside **Teradata Vantage**.

---

## 🏗️ Pipeline Architecture & Documentation

### 1. Data Ingestion (ODI)
I used **ODI** to build a robust ingestion layer. Below are the visual mappings and models that represent the data flow from source to the Bronze layer in Teradata.

#### **ODI Mapping Preview:**
![ODI Mapping](./Oracle%20Data%20Integrator/Mappings/your_mapping_image_name.png)
*(Replace 'your_mapping_image_name.png' with the actual file name in your folder)*

#### **ODI Models:**
![ODI Models](./Oracle%20Data%20Integrator/Models/your_model_image_name.png)

---

### 2. Data Transformation (SQL & Python)
The transformation logic is documented in a Jupyter Notebook. I combined the power of **SQL** for table structures and **teradataml (Python)** for data cleaning and joining the Final Gold Layer.

#### **Transformation Logic (Jupyter):**
![Jupyter Logic](./Teradata/your_jupyter_screenshot_name.png)

> **View Full Script:** [Jupyter Notebook](./Teradata/Sql_queries_in_Jupyter_python_interface.ipynb)

---

## 📂 Repository Structure
* **📁 Data Source/**: Raw CSV samples.
* **📁 Oracle Data Integrator/**: Contains exported `.xml` project and logic screenshots.
* **📁 Teradata/**: Python/SQL transformation scripts.

---

## 🛠️ Key Technical Features
* **SQL & Python Hybrid:** Using SQL for DDL and Python for complex DML.
* **In-Database Processing:** Transformations happen directly in Teradata for maximum performance.
* **Enterprise Standards:** Full use of ODI for professional ETL orchestration.

---

## 📈 Next Steps
* [ ] **Tableau Visualization:** (Work in Progress) Building the ROI & Attribution Dashboard.

---
**Contact:**
Mahmoud - [https://www.linkedin.com/in/mahmoud-mamdouh-324125220/]
