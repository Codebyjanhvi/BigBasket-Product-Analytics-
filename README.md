                                                  **BigBasket Product Analytics and Pricing Dashboard**

________________________________________
                                                                    Project Overview
This project focuses on end-to-end product and pricing analytics using a real product catalog dataset from the BigBasket online grocery platform.
The objective is to understand how BigBasket’s product assortment is structured and how pricing, discounts, brands, and categories behave across the catalog. An interactive Power BI dashboard was built to present business insights in a clear and decision-oriented manner.
The project follows the complete analytics lifecycle:
raw data → cleaning → feature engineering → exploratory data analysis → business insights → dashboarding.

                                                                    Business Problem
An online grocery company like BigBasket lacks clear visibility into:
•	Which categories and sub-categories dominate the product catalog
•	How prices vary across categories and brands
•	Which brands are positioned as premium versus budget
•	How aggressive discounting is across different categories
•	Which categories contribute the most to revenue potential
Most pricing and assortment decisions are made without structured insights from historical product data.

                                                                     Project Objectives
The key objectives of this project are:
•	Analyze product distribution across categories and sub-categories
•	Study sale price variation and price outliers
•	Identify premium and budget product segments
•	Analyze discount behavior and promotional strategies
•	Estimate category-wise revenue potential
•	Generate actionable insights for pricing and assortment optimization
________________________________________
                                                                                Dataset

                                                                                
Source: Kaggle – BigBasket Indian Grocery Dataset
The dataset contains product-level data scraped from the BigBasket website.
Dataset size:
•	27,555 product records
•	10 original columns
Key columns used:
Column Name	Description
product	Product name
category	Product category
sub_category	Product sub-category
brand	Brand name
sale_price	Discounted selling price
market_price	Original market price
rating	Customer rating
description	Product description
                                                                        Tools and Technologies Used

                                                                        
•	Python for data cleaning, feature engineering, and exploratory data analysi
•	Pandas and NumPy for data manipulation
•	Matplotlib and Seaborn for visual analysis
•	Power BI for interactive dashboard creation
•	Jupyter Notebook / Google Colab as the development environment

                                                                            Project Workflow


1. Data Ingestion
The CSV dataset was loaded into Pandas and examined for:

•	Data types
•	Number of records
•	Missing values
•	Overall structure using df.info() and df.head()


3. Data Cleaning and Preprocessing
The following preprocessing steps were performed:

•	Dropped the unnecessary index column
•	Removed rows with missing product or brand values
•	Imputed missing rating values using the median rating
•	Filled missing description values with a placeholder string
•	Standardized column names for consistency


4. Feature Engineering
New analytical columns were created to support deeper analysis:

•	discount_pct
= (market_price − sale_price) / market_price × 100
•	price_segment
Categorized into Very Low, Low, Medium, High, and Premium based on sale price ranges
•	high_discount_flag
Binary flag for products with discount percentage greater than or equal to 30 percent
•	revenue_potential
= sale_price × 1
Used as a pricing proxy per product

4. Exploratory Data Analysis
The following analyses were performed:

•	Category-wise and sub-category-wise product counts
•	Sale price distribution and outlier detection
•	Category-wise average sale price
•	Discount percentage distribution
•	Price segmentation across products

5. Business Insights Generated
Key insights derived from the analysis include:

•	Certain categories such as Fruits and Vegetables and Staples dominate the product catalog.
•	Premium brands show significantly higher average sale prices compared to mass-market brands.
•	A small subset of products contributes disproportionately to overall revenue potential.
•	Several categories exhibit aggressive discounting behavior with discount percentages above 30 percent.
•	Budget-priced products form the largest portion of the catalog.

                                                                Dashboard Overview (Power BI)

                                                                
An interactive Power BI dashboard was built with the following components:

•	KPI cards for:
o	Total number of products
o	Average sale price
o	Average discount percentage
o	Total revenue potential
•	Visuals for:
o	Category-wise product distribution
o	Brand-wise product counts
o	Category-wise revenue potential
o	Price distribution histogram
o	Top 10 most expensive products
o	Top 10 cheapest products
•	Filters and slicers for:
o	Category
o	Sub-category
o	Brand
o	Price segment

Key Business Use Cases
This dashboard can be used by business teams to:

•	Optimize pricing strategies across categories and brands
•	Identify over-discounted products
•	Improve assortment planning
•	Detect premium and budget brand positioning
•	Prioritize high-revenue-potential categories

Future Enhancements
Possible extensions of this project include:

•	Integrating sales volume data to calculate actual revenue
•	Time-series analysis using historical pricing data
•	Customer segmentation using ratings and reviews
•	Machine learning models for price and demand forecasting

