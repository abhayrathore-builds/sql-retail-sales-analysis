# Retail Sales Strategy Analysis: Uncovering Revenue Risks and Customer Retention Opportunities


## Project Background

This project analyzes a retail business selling Bikes, Accessories, and Clothing across six developed markets including the United States and Australia. Despite operating across multiple categories and geographies, the business faces two critical strategic risks — extreme revenue concentration in a single product category and weak customer retention. This analysis was conducted to help the business decide whether to diversify revenue across categories and how to improve customer retention before these risks impact long term growth.

---

## Business decisions

- Which product categories contribute the most revenue?
- Which products are the highest and lowest performers?
- How are customers segmented based on purchasing behavior?
- What is the average order value and monthly customer spending?
- What percentage does each product category contribute to total revenue?

---

## Business Insights

### 1. Bikes dominate company revenue

The Bikes category contributes **96.46%** of total revenue ($28.3M out of $29.4M), making it the primary revenue driver. Accessories (2.39%) and Clothing (1.16%) contribute only a small fraction of total sales.

---

### 2. Mountain-200 is the best-performing product line

All five highest revenue-generating products belong to the Mountain-200 family, collectively generating more than **$6.6M** in revenue, indicating exceptionally strong customer demand.

---

### 3. The United States is the largest market

With **7,482 customers**, the United States represents approximately **40%** of the total customer base—more than double Australia's **3,591 customers**—highlighting significant geographic concentration.

---

### 4. Customer retention presents a major opportunity

Approximately **79%** of customers are classified as New Customers with less than 12 months of purchasing history, while only **9%** qualify as VIP customers, indicating strong opportunities to improve customer retention and loyalty.

---

### 5. Customers purchase infrequently but spend significantly

Although the business processed **27,659 orders** across **18,484 customers**, the average customer places fewer than **1.5 orders**. However, the average order value exceeds **$1,000**, suggesting a business model driven by high-value purchases rather than frequent transactions.

---

### 6. Revenue peaked in 2013

Annual revenue increased from **$43K** in 2010 to **$16.3M** in 2013 before dropping sharply in 2014. This pattern suggests either incomplete data for 2014 or a significant business change that warrants further investigation.

---

### 7. Average selling price has steadily declined

Average selling price decreased from **$3,101** in 2010 to **$1,668** in 2014, potentially indicating a shift toward lower-priced products, increased discounting, or changes in product mix.

---

## Appendix

### Project Structure

#### Phase 1 — Exploratory Data Analysis (EDA)

The first phase focuses on understanding the dataset through:

- Database exploration
- Data quality checks
- Dimension exploration
- Measure exploration
- Magnitude analysis
- Ranking analysis
- Headline KPI calculation

#### Phase 2 — Advanced Analysis

The second phase answers key business questions using advanced SQL techniques through:

- Change over time analysis
- Cumulative analysis
- Year-over-year product performance
- Part-to-whole analysis
- Customer segmentation
- Product segmentation
- Customer Report
- Product Report

---



### Technical Skills Demonstrated

- Window Functions (`SUM`, `AVG`, `LAG`, `OVER`, `PARTITION BY`)
- Common Table Expressions (CTEs)
- Complex JOIN operations
- Aggregate Functions (`GROUP BY`, `HAVING`)
- CASE expressions for business logic and segmentation
- Subqueries and derived tables
- Views (`CREATE OR ALTER VIEW`)
- Date Functions (`DATETRUNC`, `DATEDIFF`, `YEAR`, `MONTH`)
- NULL handling (`ISNULL`, `NULLIF`)
- Data type casting
- `UNION ALL` for consolidated reporting

---

### Tools & Technologies

- Microsoft SQL Server
- SQL Server Management Studio (SSMS)
- Git
- GitHub

---

### Database Schema

The project follows a **Star Schema** consisting of one fact table and two dimension tables.

- **gold.fact_sales** — Transaction-level sales records
- **gold.dim_customers** — Customer demographics and geographic information
- **gold.dim_products** — Product, category, subcategory, and cost information

![Database Schema](images/schema.png)

---

### Reporting Views

#### Customer Report

The Customer Report provides a consolidated view of customer purchasing behavior, revenue contribution, order frequency, customer segmentation, and key customer metrics.

![Customer Report](images/customer_report.png)

---

#### Product Report

The Product Report provides a consolidated view of product performance, revenue contribution, pricing metrics, product segmentation, and sales trends.

![Product Report](images/product_report.png)
