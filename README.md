BigBasket Product Analytics & Pricing Dashboard

 End-to-End Data Analytics Project

📌 Project Overview

This project performs end-to-end product and pricing analytics using real product catalog data from the BigBasket online grocery platform.

The goal of this project is to help business stakeholders understand:

Product catalog composition

Category and sub-category distribution

Brand presence and pricing strategy

Discount patterns and promotional intensity

Revenue potential by category

Premium vs budget product positioning

The project also includes a Power BI dashboard for interactive business reporting.

Business Problem

An online grocery retailer like BigBasket lacks clear visibility into:

Which categories and sub-categories dominate the product catalog

How prices vary across categories and brands

Which brands are positioned as premium vs budget

How aggressive discounting is being applied

Which categories drive the highest revenue potential

Decisions on pricing, promotions, and assortment planning are often made without structured data insights.

🎯 Business Objectives

Analyze product distribution across categories and sub-categories

Study price variation and outliers

Identify premium vs budget product segments

Analyze discount behavior and promotional strategies

Estimate category-wise revenue potential

Generate insights for pricing and assortment optimization

📊 Dataset

Source: Kaggle – BigBasket Indian Grocery Dataset
🔗 https://www.kaggle.com/code/ridamahmood005/indian-grocery-supermarket-big-basket-eda/input

Dataset Size:

27,555 products

10 original columns

Key Columns Used:

Column Name	Description
product	Product name
category	Product category
sub_category	Product sub-category
brand	Brand name
sale_price	Discounted selling price
market_price	Original market price
rating	Customer rating
description	Product description
🛠 Tools & Technologies

Python – Data cleaning, feature engineering, EDA

Pandas, NumPy – Data manipulation

Matplotlib, Seaborn – Data visualization

Power BI – Interactive dashboard

Jupyter / Google Colab – Notebook environment

🔄 Project Workflow
1️⃣ Data Ingestion

Loaded CSV dataset into Pandas

Checked schema, data types, and missing values

2️⃣ Data Cleaning & Preprocessing

Removed unnecessary index column

Dropped rows with missing product or brand

Imputed missing ratings using median

Filled missing descriptions with placeholder values

Standardized column names

3️⃣ Feature Engineering

Created discount_pct using market price and sale price

Created price_segment (Very Low, Low, Medium, High, Premium)

Created high_discount_flag (≥ 30% discount)

Created revenue_potential as a pricing proxy

4️⃣ Exploratory Data Analysis (EDA)

Category-wise and sub-category-wise product distribution

Sale price distribution

Category-wise average price

Discount percentage distribution

Premium vs budget product segmentation

5️⃣ Advanced Product & Brand Analytics

Brand-wise product count

Brand-wise average sale price

Top 10 most expensive products

Top 10 cheapest products

High-discount product analysis

Category-wise revenue potential

6️⃣ Business Insights

A small number of categories contribute the majority of revenue potential

Clear premium and budget brand positioning exists

Price distribution is heavily right-skewed

High-discount products are concentrated in specific categories

Most products fall into low to medium price segments

7️⃣ Business Recommendations

Focus promotions on high-revenue categories

Avoid deep discounting on premium brands

Rationalize low-performing SKUs

Promote budget and mid-range products

Use category-level discount strategies

📈 Power BI Dashboard

The dashboard provides interactive views for:

Total products

Average sale price

Total revenue potential

Category-wise product count

Brand-wise product count

Category-wise revenue potential

Discount distribution

Price segmentation

📌 Key Business Impact

Identified dominant product categories and brands

Revealed premium vs budget product positioning

Highlighted aggressive discounting patterns

Estimated revenue potential by category
