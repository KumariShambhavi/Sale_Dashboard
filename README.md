# Sale_Dashboard
# 📊 Interactive Business Dashboard

## 🎯 Objective
Design a professional and interactive dashboard for business stakeholders using **Power BI** to help them make data-driven decisions.

---

## 🛠️ Tools Used
- Power BI Desktop
- DAX (Data Analysis Expressions)
- sales_data_sample.csv (Dataset)

---

## 📁 Deliverables
- ✅ **Interactive Power BI Dashboard**  
- ✅ **Summary Presentation (PPT)**  
- ✅ **README Documentation**

---

## 📌 Project Overview

This project focuses on creating a clean, insightful, and dynamic dashboard to visualize business KPIs. The dashboard aims to provide top-level executives and stakeholders with real-time business performance insights.

---

## 📂 Dataset Description

**File Name:** `sales_data_sample.csv`  
**Key Fields:**
- `ORDERDATE`: Order date of each transaction
- `SALES`: Sales revenue
- `QUANTITYORDERED`: Quantity sold
- `PRODUCTLINE`: Category of products
- `CUSTOMERNAME`, `COUNTRY`, `STATUS`, `DEALSIZE` – Customer and order info

---

## 📊 Dashboard Features

- 💰 **KPI Cards** for Total Sales, Profit, Order Volume
- 📅 **Time-Series Visuals**: Sales trends over Year/Month
- 🗺️ **Geographic Map**: Country-wise Sales Distribution
- 📦 **Category Breakdown**: Product Line Performance
- 🧠 **Interactivity**: Slicers for Year, Month, Country, ProductLine
- 🎨 **Professional Theme**: Color-coordinated visuals
- 🧭 **Navigation Buttons** (for multiple pages if needed)
- ✅ **Sorted Months** for correct chronology (Jan to Dec)

---

## 🧱 Steps to Build the Dashboard

### 1. Load Data
- Open Power BI Desktop
- Load `sales_data_sample.csv`

### 2. Create Date Table
```dax
DateTable = CALENDAR(MIN(sales_data_sample[ORDERDATE]), MAX(sales_data_sample[ORDERDATE]))
