# Project Summary
This project analyzes Zepto's product catalog and inventory data using SQL. The dataset (zepto.csv) contains detailed information about product categories, prices, discounts, availability, weights, and stock levels. The analysis focuses on data cleaning, exploration, and generating business insights to optimize pricing strategies, manage inventory, and identify revenue opportunities.
## Dataset Overview
- **Source** - Zepto CSV file (zepto.csv) was sourced from Kaggle and originally scraped from Zepto's official product listings.
- **Total Record** - Multiple thousand SKUs (exact count derived via SQL)
- **Key Columns**:
  - category – Product category
  -	name – Product name
  -	mrp – Maximum retail price
  -	discountPercent – Discount offered
  - availableQuantity – Quantity available
  - discountedSellingPrice – Price after discount
  -	weightInGms – Product weight in grams
  -	outOfStock – Stock availability flag
  -	quantity – Quantity metric for sales
  -	sku_id – Auto-incremented primary key
## Tools & Technologies Used
- **Database:** MySQL
- **Language:** SQL
- **Environment:** MySQL Workbench
## Steps Performed
### 1. **Data Exploration**
- Counted total rows and displayed sample records.
- Checked for null values.
- Identified unique product categories.
- Counted in-stock vs out-of-stock products.
### 2. **Data Cleaning**
- Removed products with `MRP = 0` or `Selling Price = 0`.
- Converted prices from paise to rupees.
- Standardized weight units.
### 3. **Data Analysis & Queries**
- **Q1:** Found Top 10 best-value products based on discount percentage.
- **Q2:** Identified High MRP products that are out of stock.
- **Q3:** Estimated revenue for each product category.
- **Q4:** Filtered expensive products (MRP > ₹500) with minimal discount.
- **Q5:** Ranked Top 5 categories with highest average discount.
- **Q6:**  Calculated Price per gram for products above 100g.
- **Q7:** Categorized products based on weight into Low, Medium and Bulk.
- **Q8:** Measured Total inventory weight per product category.
## How to Run the Project
1. Import the dataset (`zepto.csv`) into MySQL.
2. Run the SQL script `zepto-sql-data-analysis.sql` in MySQL Workbench.
3. Review query outputs for insights.
























