<h1 align="center">📊 Power BI Sales Dashboard Analysis</h1>

![Cover photo](https://github.com/user-attachments/assets/0b6c49b9-f760-4370-bc7e-89fcf6359af2)


## 📝 Project Overview

This project showcases the development of an interactive **Sales Dashboard in Power BI** using a **dirty sales dataset** that required significant cleaning and transformation before analysis.

The goal of this project was not only to build a visually appealing dashboard, but also to demonstrate the **real workflow of a data analyst**, starting from messy raw data, cleaning it in **Power Query**, modeling it properly, and turning it into useful business insights.

This project simulates a realistic retail business reporting scenario for a gadget and electronics store.

---

## 📚 Table of Contents

- [🎯 Project Objectives](#-project-objectives)
- [🗂️ Dataset Description](#️-dataset-description)
- [🧹 Data Cleaning Process](#-data-cleaning-process)
- [🧠 Data Model & Assumptions](#-data-model--assumptions)
- [📈 Dashboard Pages](#-dashboard-pages)
- [📌 Key Metrics](#-key-metrics)
- [🧮 DAX Measures Used](#-dax-measures-used)
- [🔍 Key Insights](#-key-insights)
- [💡 Recommendations](#-recommendations)
- [🖼️ Dashboard Preview](#️-dashboard-preview)
- [📂 Project Files](#-project-files)
- [🛠️ Tools Used](#️-tools-used)
- [🚀 How to Use This Project](#-how-to-use-this-project)
- [📄 Presentation Slides](#-presentation-slides)
- [⚠️ Disclaimer](#️-disclaimer)
- [🔗 Connect With Me](#-connect-with-me)

---

## 🎯 Project Objectives

The main objectives of this project were to:

- Clean and prepare a messy sales dataset for analysis
- Build an interactive dashboard in **Power BI**
- Track business performance using key sales metrics
- Analyze revenue trends over time
- Identify top-performing products and customers
- Compare sales performance across regions
- Present findings in a simple and business-friendly format

---

## 🗂️ Dataset Description

The dataset used for this project is a **simulated dirty sales dataset** designed to reflect real-world business reporting challenges.

### Dataset Features:
- Large sales transaction dataset
- Missing values in key fields
- Mixed date formats
- Inconsistent text formatting
- Duplicate-like records
- Incorrect revenue entries
- Blank customer, product, and region fields

### Main Columns Included:
- Order ID
- Order Date
- Customer Name
- Customer Segment
- Product Name
- Category
- Region
- Sales Rep
- Quantity
- Unit Price
- Revenue
- Discount
- Payment Method
- Order Status

---

## 🧹 Data Cleaning Process

Before building the dashboard, the dataset was cleaned and transformed in **Power Query**.

### Cleaning Steps Performed:
- Removed duplicate-like rows
- Standardized inconsistent text values
  - Example: `Lagos`, `lagos`, `LAGOS`
- Fixed mixed date formats
- Replaced missing values with readable placeholders
- Corrected data types
- Standardized payment method values
- Recalculated revenue where necessary
- Improved data consistency for analysis

### Examples of Placeholder Replacements:
- Blank Customer Name → `Unknown Customer`
- Blank Product Name → `Unknown Product`
- Blank Region → `Unknown State`
- Blank Sales Rep → `Unassigned`

This step was essential to ensure the dashboard outputs were accurate and presentable.

---

## 🧠 Data Model & Assumptions

### Data Model
This project was built using a **single-table sales model** for simplicity and beginner portfolio demonstration.

### Assumptions Made
To prepare the data for reporting, the following assumptions were applied:

- Revenue = `Quantity × Unit Price`
- Missing customer names were labeled as **Unknown Customer**
- Missing product names were labeled as **Unknown Product**
- Missing region values were labeled as **Unknown State**
- Missing sales reps were labeled as **Unassigned**
- Date formats were standardized to support monthly and quarterly analysis
- Inconsistent entries were cleaned for readability and reporting consistency

These assumptions helped make the data suitable for storytelling and business analysis.

---

## 📈 Dashboard Pages

This dashboard contains **three main report pages**:

### 1️⃣ Overview Page
Provides a high-level business summary including:
- Total Revenue
- Total Orders
- Average Revenue
- Quantity Sold
- Monthly Sales Trend
- Top Customers
- Top Product by Revenue

### 2️⃣ Product Analysis Page
Focuses on product performance and product-driven sales trends:
- Top Product by Quantity Sold
- Top Product by Revenue
- Product Performance by Region

### 3️⃣ Customer Analysis Page
Focuses on customer contribution and regional customer activity:
- Top Customers by Orders
- Revenue by Region
- Regional Customer Performance

---

## 📌 Key Metrics

The dashboard includes the following core KPIs:

- **Total Orders**
- **Total Revenue**
- **Average Revenue**
- **Quantity Sold**

Additional performance metrics include:
- Monthly Sales Trend
- Revenue by Region
- Top Products by Revenue
- Top Products by Quantity
- Top Customers by Revenue
- Top Customers by Orders

---

## 🧮 DAX Measures Used
- `Total Revenue = SUM(Sales[Revenue])`
- `Total Orders = COUNT(Sales[Order ID])`
- `Quantity Sold = SUM(Sales[Quantity])`
- `Avg Revenue = DIVIDE([Total Revenue], [Total Orders], 0)`
- `Month Name = FORMAT(Sales[Order Date], "MMMM")`
- `Month Number = MONTH(Sales[Order Date])`
- `Year Month = FORMAT(Sales[Order Date], "YYYY-MMM")`
- `Quarter = "Q" & FORMAT(Sales[Order Date], "Q")` 
 
---
## 🔍 Key Insights

Some high-level observations from the dashboard include:

- Sales performance can be tracked clearly across time using monthly trend visuals
- A few products contribute significantly to total revenue
- Certain customers contribute more consistently than others
- Regional performance varies across the business
- Data cleaning significantly improved report quality and usability

---
## 💡 Recommendations

Based on the dashboard structure and analysis approach, the following actions are recommended:

- Focus on top-performing products for stronger revenue generation
- Monitor customer purchasing patterns for retention opportunities
- Use regional performance trends for location-based strategy
- Improve data entry processes to reduce inconsistencies and missing values
- Standardize business records to improve reporting accuracy

  ---
## 🖼️ Dashboard Preview
📍 Overview Page

<img width="603" height="333" alt="Overview page png" src="https://github.com/user-attachments/assets/666ee84b-f984-4b36-86f5-338b3fd8a829" />

--- 
📍 Product Analysis Page

<img width="601" height="341" alt="Product Analysis page png" src="https://github.com/user-attachments/assets/602bc7aa-53fd-496e-b411-1ab23bf738ca" />

---
📍 Customer Analysis Page

<img width="600" height="336" alt="Customer Analysis page png" src="https://github.com/user-attachments/assets/3d7db713-c190-49ca-8faa-fdf0d2c5b253" /> 

---
## 📂 Project Files

This repository contains:

- data/Dirty_Sales_950.csv → Raw dataset
- dashboard/Typayhub_Sales_Dashboard.pbix → Power BI dashboard file
- presentation/Typayhub_Sales_Dashboard_Presentation.pptx → Project presentation slides
- images/ → Dashboard screenshots
- README.md → Project documentation

---
## 🛠️ Tools Used

The following tools were used in this project:

- Microsoft Power BI
- Power Query
- DAX
- Microsoft Excel
- PowerPoint
 -GitHub

  ---
## 🚀 How to Use This Project

To explore this project:

- Download the dataset from the data/ folder
- Open the .pbix file in Power BI Desktop
- Explore the report pages and visuals
- Review the PowerPoint presentation for project walkthrough
- Read the README for project context and methodology

  ---
## 📄 Presentation Slides

The full presentation slides for this project are included in this repository:

📁 presentation/Typayhub_Sales_Dashboard_Presentation.pptx

This presentation contains:

- project overview
- dashboard explanation
- cleaning process
- key metrics
- insights
- recommendations
- report usage guide

  ---
## ⚠️ Disclaimer

This project was developed as a portfolio and learning project using a simulated retail sales dataset.

# Important Notes:
- The dataset is not from a real company
- The business name and records are used for demonstration purposes
- Some values were intentionally dirty to simulate real-world data cleaning challenges
- This project is intended to showcase practical analytics workflow and reporting skills
🙌 Author

## 🔗 Connect With Me

You can also connect with me on LinkedIn and follow my analytics journey  @https://www.linkedin.com/in/kelvin-etisi-39704a259/overlay/contact-info

## ⭐ If you found this project interesting

Feel free to star this repository and check out my other projects.





