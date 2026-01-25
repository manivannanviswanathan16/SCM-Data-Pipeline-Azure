# SCM-Data-Pipeline-Azure

# Automated SCM Fulfillment & Logistics Pipeline
**Domain:** Supply Chain Management | **Stack:** Azure, Databricks (PySpark), Power BI, Logic Apps

## 📌 Project Overview
As an Operations Manager, I identified a need for real-time visibility into shipping delays. This project builds a fully automated data pipeline that transforms messy, multi-source CSV data into an interactive SCM Bottleneck Dashboard.

## 🏗️ Architecture (Medallion Pattern)
- **Bronze Layer:** Raw data ingestion from Outlook Emails via **Azure Logic Apps**.
- **Silver Layer:** Schema standardization (53 to 51 columns) and deduplication using **PySpark**.
- **Gold Layer:** Business logic applied (Late Delivery Risk, Shipping Variance) stored in **Delta Tables**.



## 🚀 Key Features
- **Automated Ingestion:** Event-driven trigger that picks up SCM attachments from emails.
- **Data Governance:** Automated cleaning of "ghost columns" and schema enforcement.
- **KPI Tracking:** Real-time monitoring of "Scheduled vs. Real" shipping days.

## 📊 Dashboard Preview
> **Insight:** Identified that [Category Name] had a 1.5-day variance in shipping, leading to targeted warehouse process improvements.

<img width="2308" height="1303" alt="Screenshot 2026-01-22 153152" src="https://github.com/user-attachments/assets/663d32bd-1cdf-463e-a8ec-adcf76bc39c6" />

