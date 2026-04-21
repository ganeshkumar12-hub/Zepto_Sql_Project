# 🛒 Zepto E-commerce SQL Data Analyst Portfolio Project

This is a complete, real-world SQL data analyst portfolio project based on an e-commerce inventory dataset scraped from Zepto. The project simulates real analyst workflows — from raw data exploration to business-driven insights.

---

## 📌 Project Overview

The objective of this project is to replicate how data analysts in e-commerce and retail industries use SQL to:

- Set up a structured database from raw data  
- Perform Exploratory Data Analysis (EDA)  
- Clean and transform messy data  
- Generate business insights using SQL queries  

---

## 🎯 Key Features

- 📊 End-to-end SQL project  
- 🧹 Real-world data cleaning  
- 🔍 Exploratory data analysis  
- 📈 Business insights generation  
- 💼 Interview-ready portfolio project  

---

## 📁 Dataset Description

The dataset is sourced from Kaggle and represents product listings from Zepto.

Each row corresponds to a unique SKU (Stock Keeping Unit).

### 🧾 Columns

- `sku_id` – Unique product ID (Primary Key)  
- `name` – Product name  
- `category` – Product category  
- `mrp` – Maximum Retail Price (₹)  
- `discountPercent` – Discount percentage  
- `discountedSellingPrice` – Final selling price (₹)  
- `availableQuantity` – Units available  
- `weightInGms` – Product weight  
- `outOfStock` – Stock availability (TRUE/FALSE)  
- `quantity` – Units per package  

---

## 🛠️ Tech Stack

- PostgreSQL  
- pgAdmin  
- SQL  

---

## 🔧 Project Workflow

### 1️⃣ Database & Table Creation

```sql
CREATE TABLE zepto (
  sku_id SERIAL PRIMARY KEY,
  category VARCHAR(120),
  name VARCHAR(150) NOT NULL,
  mrp NUMERIC(8,2),
  discountPercent NUMERIC(5,2),
  availableQuantity INTEGER,
  discountedSellingPrice NUMERIC(8,2),
  weightInGms INTEGER,
  outOfStock BOOLEAN,
  quantity INTEGER
);
