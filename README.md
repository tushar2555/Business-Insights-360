# AtliQ Hardware Business Insights 360

## Project Overview

AtliQ Hardware is growing rapidly in the recent years, and they have decided to implement the data analytics using PowerBi in their company for the first time to surpass their competitors in the market and to make data driven decisions. This project is hoped to give answers to the questions of stakeholder in terms all the aspects like finance, sales, marketing and supply chain.

This project, part of the **Codebasics Bootcamp**, focuses on building an **interactive dashboard** that answers key stakeholder questions across:  
- Finance  
- Sales  
- Marketing  
- Supply Chain  
- Executive  
- Product

**Live Dashboard:** [Click here](https://app.powerbi.com/view?r=eyJrIjoiMjJkOGZkMGEtZWQ2Yy00ZWY3LWEyMjMtNjg4ZWU2NWIyNzk0IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

## Tech stacks

- SQL
- PowerBi Desktop
- Excel
- DAX language
- DAX studio (for optimizing the report)

## PowerBI techniques Learnt

- Data cleaning and transformations with **Power Query**  
- **Snowflake data modeling** for efficient relationships  
- Creating **measures and KPIs** using DAX  
- **Dynamic titles** that respond to applied filters  
- **Conditional formatting** with icons and colors  
- **Bookmarks & navigation buttons** for smooth report flow  
- **Drill-through** and **tooltips** for detailed insights  
- **Date table creation** using M language  
- **KPI indicators** for quick performance checks  
- **Data validation techniques** to ensure accuracy  
- And more 

## Company’s back ground

AltiQ hardware is a company which has grown vastly in the recent years, and opened business all over the globe. It is a company which sells, computer and computer accessories through three mediums/channel

- Retailers
- Direct
- Distributors

Recently the company has faced a unforeseen loss by opening store in America based on the surveys, intuition and some excel analysis and also the company’s competitors has handful of analytics team to perform analysis and make data driven decision. So, the AltiQ hardware has no other option other than building their analytics team for data driven insights and decisions in the future to survive better in the industry. 


### Dataset **Understanding.**

Understanding what data is available will be more helpful while doing analysis. before jumping on to the analysis get good understanding of what are data available.

Dimension table : It will have the static data like details of customer and products

Fact table : It will have the data about the transactions  

- gdb041:
    - dim_customer
        - **27** distinct markets (ex India, USA, spain)
        - **75** distinct customers thorough out the market
        - **2** types of platforms
            - Brick & Motors - Physical/offline store
            - E-commerce - Online Store (Amazon, flipkart)
        - Three channels
            - Retailer
            - Direct
            - Distributors
    - dim_market
        - **27** distinct markets (ex India, USA, spain)
        - 7 sub-zones
        - 4 regions
            - APAC
            - EU
            - nan
            - LATAM
    - dim_product
        - Divisions
            - P & A
                - Peripherals
                - Accessories
            - PC
                - Notebook
                - Desktop
            - N & S
                - Networking
                - Storage
        - There are 14 different categories, Like Internal HDD, keyboard
        - There are different variants available for the same product
    - fact_forecast_monthly
        - This table is used to forecast the customer’s need in advance, which can help in
            - Higher customer satisfaction
            - Reduced cost in warehouses for storage purpose
        - The table is denormalized by data engineering team, as it is a data warehouse which is aimed to be used for analytical work.
        - All the date of the month will be replaced by the start date of the month
        - It will have all the column names and in the end it will have the forecast quantity need of the customer
    - fact_sales_monthly
        - This table is more or less is same as fact_forecase_monthly table, but the last column has the value of sold quantity instead of forecast value.
- gdb056
    - freight_cost
        - This table has details of travel cost and other cost for each market with fiscal year
    - gross_price
        - Has the details of gross prices with product code
    - manufacturing_cost
        - Has the details of manufacturing cost with product code with year
    - Pre_invoice_dedutions
        - Has the details of pre invoice deductions percentage for each cutomer with year
    - Post_invoice_deductions
        - Post invoice deductions and other deductions details

## Dashboard Overview  

The dashboard provides a 360° view of AtliQ Hardware’s business operations across multiple domains:  

- **Home View** – Navigate seamlessly with a central landing page  
- **Finance View** – Analyze P&L statements, Net Sales trends, and top/bottom customers & products  
- **Sales View** – Explore customer and product performance with Net Sales, Gross Margin %, unit economics, and deductions  
- **Marketing View** – Gain insights by market, region, product, and customer, tracking GM% and NP% across segments  
- **Supply Chain View** – Track Forecast Accuracy, Net Error, and Absolute Error with trend analysis for optimization  
- **Executive View** – Monitor performance at a glance with revenue by division, customer, product, and channel  
- **Product View** – Identify top/bottom products by YoY GM% growth, top markets by revenue, and post-discount % trends per customer


## Data Model
The dashboard is powered by a well-structured Snowflake schema for efficient querying and optimized performance.  

![Data Model](https://github.com/tushar2555/Business-Insights-360/blob/main/Images/Data%20Model.jpg)

---

## Home Page
Central navigation hub with buttons to access each domain view.  

![Home Page](https://github.com/tushar2555/Business-Insights-360/blob/main/Images/Home%20Page.jpg)

---

## Finance View
Analyze Profit & Loss statements, Net Sales trends, and top/bottom customers & products.  

![Finance View](https://github.com/tushar2555/Business-Insights-360/blob/main/Images/Finance%20View.jpg)

---

## Sales View
Customer and product performance with insights into Net Sales, Gross Margin %, and unit economics.  

![Sales View](https://github.com/tushar2555/Business-Insights-360/blob/main/Images/Sales%20View.jpg)

---

## Marketing View
Market, region, product, and customer insights while tracking GM% and NP% across segments.  

![Marketing View](https://github.com/tushar2555/Business-Insights-360/blob/main/Images/Marketing%20View.jpg)

---

## Supply Chain View
Track Forecast Accuracy, Net Error, and Absolute Error with trend analysis for supply chain optimization.  

![Supply Chain View](https://github.com/tushar2555/Business-Insights-360/blob/main/Images/Supply%20Chain%20View.jpg)

---

## Executive View
High-level performance overview including revenue by division, customers, products, and channels.  

![Executive View](https://github.com/tushar2555/Business-Insights-360/blob/main/Images/Executive%20View.jpg)

---

## Product View
Insights into top/bottom products by YoY GM% growth, top markets by revenue, and post-discount % trends per customer.  

![Product View](https://github.com/tushar2555/Business-Insights-360/blob/main/Images/Product%20View.jpg)

## Project Outcome  

This project demonstrates how **1.5M+ rows of raw data** were transformed into an **interactive, decision-focused dashboard**.  

It enables:  
- **Finance Teams** → Monitor profitability and sales performance.  
- **Sales & Marketing Teams** → Identify key customers, products, and markets.  
- **Supply Chain Teams** → Track forecast accuracy and optimize planning.  
- **Executives** → Make smarter and faster decisions with confidence.  
