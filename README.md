# Automotive-Sales
Seles Performance & Total Quotations report 

An end-to-end **Power BI analytics project** focused on transforming raw automotive quotation data into **actionable executive insights**.

This project covers the full analytics lifecycle:  
**Data collection → Data modeling → DAX calculations → Interactive dashboards → Business insights**.

---

## 📌 Project Overview
The goal of this project is to analyze automotive sales quotations and bank approvals to support:
- Executive decision-making
- Sales performance evaluation
- Banking efficiency analysis
- Product and pricing optimization

The dashboard is designed for **top management**, offering a clear and interactive overview of business performance.

---

## 📊 Data Sources
The data used in this project was collected from **multiple systems**, simulating a real-world business environment:

- 🗄️ Local ERP system (on-premise transactional data)
- ☁️ Odoo ERP (sales & operational data)
- 📄 Excel / CSV reference files

All sources were integrated into a unified analytical model.

---

## 🔄 Data Processing (ETL)
Data preparation was handled using **Power Query**, including:
- Data extraction from different sources
- Cleaning and standardization
- Handling nulls, duplicates, and inconsistent formats
- Aligning keys across systems
- Building a single, scalable fact table

---

## 🧱 Data Model
The data model follows a **star schema approach**:
- Fact table for quotations and sales
- Dimension tables for:
  - Date
  - Sales
  - Bank
  - Product (Brand / Model / Tier)
  - Channel
  - Location

This structure ensures performance, scalability, and accurate calculations.

---

## 🧮 DAX Measures
A dedicated **Measures Table** was created to organize all calculations.

Key measures include:
- Total Quotations
- Approved Quotations
- Approval Rate %
- Rejection Rate %
- Total Sales Value
- Approved Sales Value
- Average Bank Approval Time
- Performance by Brand, Model, Bank, and Salesperson

Example:
```DAX
Approval Rate % =
DIVIDE(
    [Approved Quotations],
    [Total Quotations]
)
