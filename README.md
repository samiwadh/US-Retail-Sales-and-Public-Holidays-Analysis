# 📊 US Retail Sales and Public Holidays Analysis

**Authors:** Abdul Sami (Mat: 939542), Davina David (Mat: 946851)  
**Course:** Data Management Project  
**Date:** 10 February 2026  

---

## 📌 Project Overview

This project analyzes the relationship between **US retail sales and public holidays (2014–2017)** by integrating real-world transaction data with official holiday records.

The main objective is to understand how public holidays influence customer purchasing behavior and whether holiday information improves analysis and forecasting.

The project follows a complete end-to-end data pipeline:
**data acquisition → data cleaning → integration → database storage → exploratory data analysis → insights**

---

## 🎯 Objectives

- Analyze the impact of public holidays on daily retail order volumes  
- Compare sales behavior on holiday vs non-holiday periods  
- Identify which holidays drive the highest demand  
- Evaluate whether holiday features improve prediction insights  

---

## 📂 Datasets

### 🛒 Retail Orders Dataset
- Source: Kaggle dataset  
- Time period: 2014–2017  
- Records: 9,994 orders  
- Key features: Order ID, Order Date, Customer ID, Product ID, Sales, Quantity  

### 🎉 Public Holidays Dataset
- Source: Nager.Date API  
- Records: 52 unique US public holiday dates  
- Key features: Date, Holiday Name, Country Code  

---

## ⚙️ Project Workflow

### 1. Data Acquisition
- Merged multiple yearly retail CSV files into one dataset  
- Retrieved US public holidays using API (2014–2017)  

### 2. Data Cleaning
- Removed duplicate holiday entries  
- Standardized date formats  
- Handled missing values (none in key fields)  
- Unified column naming conventions  

### 3. Data Integration
- Merged datasets using Order Date = Holiday Date  
- Created new features:
  - `IsHoliday` (binary indicator)  
  - `Holiday Name`  

---

### 4. Database Storage
- Stored final dataset in **SQLite database**
- Enabled structured SQL queries for validation and analysis  

---

### 5. Exploratory Data Analysis (EDA)

#### Research Questions:
- Do public holidays affect retail sales?
- Are orders higher on holidays?
- Which holidays drive maximum sales?
- Does holiday data improve forecasting?

---

## 📈 Key Insights

- Public holidays significantly affect customer ordering behavior  
- Higher order volumes are observed during holidays  
- Major holidays like **Christmas, Thanksgiving, and Labour Day** show strong demand spikes  
- Adding holiday features improves analytical understanding of sales patterns  

---

## 🧰 Tools & Technologies

- Python 🐍  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- SQLite (DBMS)  
- Jupyter Notebook  
- Nager.Date API  

---


---

## 📊 Results Summary

- Total orders analyzed: **9,994**
- Holiday records: **52**
- Orders on holidays: **450 (4.5%)**
- Strong demand spikes observed during major holidays  

---

## 🚀 Key Contribution

This project demonstrates a complete **data management and analysis pipeline**, including:

- Data integration from multiple sources  
- API-based enrichment  
- Database storage using SQLite  
- Business-focused exploratory analysis  

---

## 📌 Conclusion

This project shows that **public holidays have a measurable impact on retail demand patterns**, and integrating holiday information improves analytical insights.

---

## 👤 Author

**Abdul Sami**  
University of Milano-Bicocca  

