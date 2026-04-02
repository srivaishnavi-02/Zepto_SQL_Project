# Zepto_SQL_Project
Analyzed real-world e-commerce inventory data using SQL to perform data cleaning, EDA, and derive actionable business insights on pricing, inventory, and revenue.

📌 Overview

This project simulates a real-world data analyst workflow in the e-commerce domain using SQL. It focuses on working with messy inventory data, performing data cleaning, and extracting meaningful business insights.

The goal is to demonstrate how raw product-level data can be transformed into actionable insights related to pricing, inventory management, and revenue generation.

📁 Dataset

The dataset is sourced from Kaggle and is based on product listings scraped from Zepto.

Each row represents a unique SKU (Stock Keeping Unit)
The dataset reflects real-world complexity where:
Products appear multiple times with variations (size, weight, discounts)
Pricing and availability vary across listings
🧾 Key Columns
sku_id – Unique product identifier
name – Product name
category – Product category (Fruits, Snacks, Beverages, etc.)
mrp – Maximum Retail Price (converted from paise to ₹)
discountPercent – Discount applied
discountedSellingPrice – Final selling price
availableQuantity – Inventory count
weightInGms – Product weight
outOfStock – Stock availability flag
quantity – Units per package
🛠️ Tech Stack
Database: PostgreSQL
Language: SQL
Tools: pgAdmin, Git, GitHub
⚙️ Project Workflow
1. Database Setup
Designed and created a structured SQL table
Defined appropriate data types and constraints
2. Data Import
Imported dataset using pgAdmin
Resolved encoding issues by converting data to UTF-8 format
3. Data Exploration (EDA)
Analyzed dataset structure and size
Identified null values and inconsistencies
Explored product categories and stock distribution
Detected duplicate product entries across SKUs
4. Data Cleaning
Removed invalid records (zero pricing values)
Converted price columns from paise to rupees
Improved overall data consistency and usability
5. Business Analysis

Performed SQL queries to generate insights such as:

Top discounted products
High-value products that are out of stock
Revenue estimation by category
Premium products with low discounts
Categories with highest average discounts
Price-per-gram analysis for value comparison
Product segmentation based on weight
Inventory distribution across categories
📊 Key Insights
Pricing inconsistencies can significantly impact perceived value
Inventory gaps exist in high-MRP product segments
Certain categories consistently offer higher discounts
Price-per-unit analysis helps identify cost-efficient products
▶️ How to Run
Clone the repository
git clone https://github.com/your-username/zepto-sql-project.git
cd zepto-sql-project
Open the SQL file
zepto_SQL_data_analysis.sql
Create a PostgreSQL database
Run table creation queries
Import dataset
Use pgAdmin import tool
Ensure file is in UTF-8 format
Execute SQL queries for analysis
