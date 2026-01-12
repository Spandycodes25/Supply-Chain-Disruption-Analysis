# Supply Chain Disruption Analysis using Power BI

## Project Overview

Supply chain inefficiencies—particularly delivery delays—have a direct impact on customer satisfaction and business profitability.  
This project focuses on analyzing supply chain disruptions using **Business Intelligence (BI)** techniques and **Power BI dashboards** to identify the root causes of delivery delays and evaluate their impact on profitability.

The analysis provides multi-dimensional insights across:
- Products  
- Customers  
- Regions  
- Sales teams  
- Store locations  
- Time (year, quarter, month)  

The goal is to support **data-driven decision-making** that improves delivery performance, operational efficiency, and overall profitability.

---

## Objectives

- Identify key factors contributing to delivery delays  
- Analyze late delivery risk across product categories and shipping methods  
- Evaluate profitability per order  
- Perform year-over-year performance comparisons  
- Provide geographic insights at region, state, and city levels  
- Enable interactive, real-time exploration using Power BI  

---

## Tools & Technologies

- **Power BI Desktop** – Dashboard creation and DAX measures  
- **Microsoft Excel** – Data preprocessing and cleaning  
- **Star Schema Data Model** – Fact and dimension tables  
- **DAX** – Measures for profitability, delivery performance, and trends  

---

## Dataset Description

The dataset follows a **star schema** design, consisting of a **central fact table** and supporting **dimension tables**, **enabling efficient analytical querying**.

---

## Fact Table

### FactTable (Transactional Sales Data)

Contains measurable business events and links to all dimension tables.

**Key fields include:**
- OrderNumber  
- OrderDate, ShipDate, DeliveryDate  
- Sales Channel  
- Order Quantity  
- Discount Applied  
- Unit Price, Unit Cost  
- Foreign Keys: `_CustomerID`, `_ProductID`, `_SalesTeamID`, `_StoreID`  

**This table is used to compute:**
- Delivery delays  
- Profit and loss  
- Order-to-shipping intervals  
- Late delivery risk  

---

## Dimension Tables

### Dim_Customers
- Customer identifiers and details  
- Supports customer-level performance and segmentation analysis  

### Dim_Products
- Product identifiers and attributes  
- Enables product-wise sales, profitability, and delay analysis  

### Dim_Regions
- Geographic hierarchy: Region → State → City  
- Used for spatial and regional performance comparisons  

### Dim_SalesTeams
- Sales team details and region assignments  
- Enables evaluation of sales team performance and efficiency  

### Dim_StoreLocations
- Store identifiers and geographic location details  
- Used for store-level delivery and demand analysis  

---

## Data Model Architecture

- Star schema design  
- Central fact table connected to multiple dimension tables  
- Optimized for:
  - Faster query performance  
  - Simplified DAX calculations  
  - Scalable BI reporting  

---

## Power BI Dashboards & Analysis

The Power BI report includes the following analytical views:
- Home Dashboard – High-level KPIs and filters  
- Customer Analysis – Retargeting and purchasing patterns  
- Product Insights – Best-selling and delayed products  
- Location Analysis – Regional, state, and city-level insights  
- Sales Team Analysis – Team-wise contribution and efficiency  
- Transaction Analysis – Order volume, discounts, and margins  
- Time Analysis – Monthly, quarterly, and yearly trends  

Each dashboard supports **interactive filtering and drill-downs**.

---

## Key Insights Generated

- Identification of regions with higher delivery delays  
- Product categories contributing most to late deliveries  
- Relationship between discounts, profit margins, and delays  
- Sales team and store-level performance differences  
- Year-over-year supply chain efficiency trends  

---

## Learning Outcomes

- Practical implementation of Business Intelligence concepts  
- Hands-on experience with Power BI and DAX  
- Designing analytical models using fact and dimension tables  
- Translating raw data into actionable business insights  

---

## Future Enhancements

- Integration of real-time data sources  
- Predictive modeling for delivery delay risk  
- Supplier-level disruption analysis  
- AI-driven anomaly detection and forecasting  

---

## References

- Cumano, Z., & Sharma, B. (2022). Supply Chain Analytics with Power BI  
- Brintrup et al. (2020). Predicting Supplier Disruptions  
- Powell, B. (2018). *Mastering Microsoft Power BI*  
- Seamark, P. (2018). *Beginning DAX with Power BI*  

---

## Authors

- Yash Rade  
- Atharva Suryawanshi  
- Spandan Surdas  

Under the guidance of **Prof. Dr. Rahul Patil**  
Department of Computer Engineering  
Pimpri Chinchwad College of Engineering
