📊 Sales Data Analysis — Interactive Power BI dashboard for revenue, profit, and growth analysis.

![License](https://img.shields.io/badge/License-MIT-blue)
![Power BI](https://img.shields.io/badge/Tool-Power%20BI-orange)

A complete end-to-end Sales Analytics project designed to transform raw sales data into meaningful insights. This dashboard provides a clear view of sales trends, revenue performance, customer segments, product profitability, regional growth patterns, and KPI tracking to support strategic business decision-making.

🚀 Project Overview

This project analyzes historical sales data to uncover key business metrics such as total revenue, sales by region, product category performance, customer purchasing patterns, and time-based sales trends.
The goal is to help stakeholders make data-driven decisions that improve revenue, optimize product strategy, and boost operational efficiency.

📷 Dashboard Preview:

<a href="https://github.com/MReza07/Sales-Data-Analysis/blob/main/Schreenshots/Sales%20Report.PNG">View Dashboard</a>

## Key Metrics Overview:
Displays total revenue, total cost, total units sold, gross profit, and gross profit percentage.
​
Yearly Revenue Analysis: Visualizes total revenue by year and breaks it down by product names and subcategories.
​
Category Revenue Distribution: Highlights revenue contributions from different categories (e.g., Special and General).

Top Sales Representatives: Identifies the top-performing sales reps based on revenue generated.

Quarterly and Monthly Growth Trends: Tracks quarter-to-quarter (QtQ) and month-over-month (MOM) growth percentages for revenue and gross profit. 
​
Detailed Revenue Trends: Provides granular revenue data by date, month, and year for deeper analysis. ​
## Dataset
<a href="https://github.com/MReza07/Sales-Data-Analysis/tree/main/Dataset">Download Dataset<a/>

## data dictionary

ProductID	ProductName	Date	Units	RevenueDiscount	Category	Sales Rep Name	ProductName	RetailPrice	StandardCost
4	Alder	2.1.2014	145	0.55	Special	Jan Novotny	Alder	23.95	7.55
9	Linder	2.1.2014	142	0.55	General	John White	Linder	23.95	7.55
2	Magnum	2.1.2014	135	0.55	General	Ellen Woody	Magnum	23.95	7.55
10	Quad	2.1.2014	133	0.55	General	Mark Spancer	Quad	43.95	13.75
3	Black Monk	2.1.2014	133	0.55	General	Ellie Gill	Black Monk	43.95	13.75
9	Quad	2.1.2014	133	0.55	General	Bill Muray	Quad	43.95	13.75
5	Bing	2.1.2014	131	0.55	General	El Bob	Bing	26.95	8.25
6	VanHelen	2.1.2014	119	0.55	General	Jan Novotny	VanHelen	26.95	8.25
11	Magnum	2.1.2014	118	0.55	Special	John White	Magnum	26.95	8.25
3	Carlota	2.1.2014	117	0.55	Special	Ellen Woody	Carlota	29.95	9.15
5	Carlota	2.1.2014	117	0.55	Special	Mark Spancer	Carlota	29.95	9.15
6	Bing	2.1.2014	114	0.55	Special	Ellie Gill	Bing	26.95	8.25
10	Carlota	2.1.2014	112	0.55	Special	Bill Muray	Carlota	29.95	9.15
<img width="1395" height="337" alt="image" src="https://github.com/user-attachments/assets/57633f49-00f8-4529-94cd-4886af5a6a18" />


## Data Highlights

Total Revenue: $126M ​

Total Cost: $40M ​

Total Units Sold: 4M ​

Gross Profit: $87M (69% Gross Profit Percentage) ​

Revenue Growth: QtQ growth peaked at 36.67% in Q1 2017. ​


## Visualizations

The dashboard includes:

Bar Charts: For yearly revenue and product/subcategory breakdowns. ​

Pie Charts: For category revenue distribution.

Line Graphs: For QtQ and MOM growth trends.

Tables: For detailed revenue and profit data by date, month, and year.

## 🛠️ Tools & Technologies

Power BI Desktop – Data modeling, visualization, DAX

Excel / CSV – Data sources

Power Query – Data cleaning & transformation

DAX Measures – KPI formulas and advanced calculations​

## 📁 Project Structure

│── Data/

│     └── Dataset.xlsx

│── PBIX/
│     └── Sales Data Analysis.pbix

│── Schreenshots/

│     └── Sales Report png

│── README.md


## 📊 Dashboard Features

Interactive filters for Region, Product, Customer Segment, Year, Category

Drill-through pages for product-level and customer-level analysis

Visual KPIs:

Total Sales

Total Profit

Total Quantity Sold

Average Discount

YoY Growth

Comparison charts: Actual vs Target Sales

Trend charts for monthly and quarterly patterns

Regional maps for geographic sales insights

## 📐 Sample DAX Measures

Total Sales = SUM('Sales'[SalesAmount])

Total Profit = SUM('Sales'[Profit])


YoY Growth % = 
VAR CurrentYear = CALCULATE([Total Sales], YEAR('Sales'[OrderDate]) = MAX(YEAR('Sales'[OrderDate])))
VAR LastYear = CALCULATE([Total Sales], YEAR('Sales'[OrderDate]) = MAX(YEAR('Sales'[OrderDate])) - 1)
RETURN DIVIDE(CurrentYear - LastYear, LastYear)

## 🧠 Key Outcomes

Identified top-selling regions and products contributing most to revenue

Highlighted loss-making products with high discount dependency

Revealed seasonal peaks such as Q4 sales boost

Shown customer segment insights to support targeted marketing

Provided actionable insights for pricing, promotions, and inventory planning

## How to Open

1. Clone repo
   git clone https://github.com/MReza07/Sales-Data-Analysis.git
2. Open `PBIX/Sales Data Analysis.pbix` in Power BI Desktop (latest).
3.  Go to Home → Transform Data → Refresh to load latest dataset.
4. If prompted, update data source to `Dataset/Dataset.xlsx` then Refresh.


## 📜 License

This project is released under the MIT License.

Contributions are welcome! Please submit a pull request or open an issue for any suggestions or improvements.

## 👤 Contact

For collaboration or dashboard development:

📧 Email:reazulrepon@gmail.com

💼 GitHub profile link-https://github.com/MReza07
