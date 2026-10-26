# Restaurant Sales & Waste Reduction Analysis

## Table of contents
- [Project Overview](#project-overview)
- [Business Problem](#Business-Problem)
- [Project Objectives](#project-Objectives)
- [Dataset](#DDataset)
- [Methdology](#project-overview)
- [Key Performance Reslts](#Key-Performance-Results)
- [Key Insight](#Key-Insights)
- [Strategic Reccomendations](#Strategic-Reccomendations)
- [Expected Business Impact](#Expected-Business-Impact)
- [Project Limitation](#project-Limitation)
- [Future Improvement](#Future-Improvement)
- [Tools Used](#Tools-Used)
- [Skills Demostrated](#Skills-Demonstrated)
- [Project Outcome](#project-Outcome)
- [About the Analyst](#About-the-Analyst)



## Project Overview

Food waste is one of the hidden operational costs in the restaurant industry. While sales reports can show how much a restaurant sells, they do not necessarily reveal how much inventory is being wasted or how that waste affects profitability.

This project combines **restaurant sales data with simulated inventory and waste data** to investigate the relationship between customer demand, production, waste, and profitability.

Using **Power BI, Power Query, DAX, and Microsoft Excel**, I transformed raw transactional data into an interactive business intelligence dashboard designed to help restaurant managers:

* Identify high-waste products
* Understand waste patterns throughout the day
* Compare sales performance against waste
* Detect potential overproduction
* Evaluate underperforming menu items
* Improve inventory planning
* Reduce operational losses
* Make more informed production and menu decisions

The central objective was to move beyond **"What are we selling?"** and investigate **"Where are we losing money operationally?"**

---

# Business Problem

Restaurants can experience significant losses through:

* Overproduction
* Poor inventory planning
* Excessive food waste
* Inefficient production schedules
* Poor-performing menu items
* Misalignment between production volume and customer demand

Traditional sales reporting may identify which products generate the most revenue, but it does not necessarily explain whether those products are being produced efficiently.

#  Project Objectives

The dashboard was designed to answer the following business questions:

1. Which menu items generate the highest waste cost?
2. Which products have the highest waste percentage?
3. At what time of day does the restaurant experience the highest waste?
4. Which products are selling well but also generating excessive waste?
5. Which products generate high waste with relatively low sales?
6. How much does waste cost the business?
7. Which menu items require further operational review?
8. What operational changes could reduce waste and improve profitability?

---

# Dataset

## Source Sales Dataset

The primary sales data was sourced from the **Balaji Restaurant Sales Dataset on Kaggle**.

The dataset contains transactional sales information including:

* Order ID
* Item Name
* Quantity
* Order Date
* Time of Sale
* Revenue

## Simulated Inventory & Waste Dataset

The original sales dataset did not contain inventory or waste information.

To enable an operational waste analysis, I created a **simulated inventory/waste dataset** containing:

* Product Name
* Quantity Produced
* Quantity Sold
* Quantity Wasted
* Waste Cost
* Waste Percentage

The simulated data was designed to represent realistic operational waste patterns that could occur in a fast-food restaurant environment.

---

# Methodology

The project followed a structured data analytics workflow from raw data preparation through business recommendations.

 1. Data Collection
 2. Data Cleaning & Preprocessing
 3. Data Transformation
 4. Data Modelling
 5. KPI Development
 6. Exploratory Analysis
 7. Dashboard Development

# Key Performance Results

The dashboard revealed the following overall performance:

| KPI                          | Result |
| ---------------------------- | -----: |
| **Total Sales**              | ~$275K |
| **Total Margin**             | ~$161K |
| **Total Waste Cost**         |  >$14K |
| **Overall Waste Percentage** |   ~11% |

---

# Key Insights

 1. Waste Is Concentrated Among Certain Products

Several products contribute disproportionately to waste costs despite only moderate sales performance.

 2. Waste Is Higher During Earlier Operating Hours

The time-of-day analysis showed that waste was highest during earlier operating periods before gradually declining throughout the day.

This pattern may indicate that some food is being prepared before sufficient customer demand has materialized.

 3. Some Products Show a Production–Demand Mismatch

 4. High Sales Does Not Automatically Mean High Efficiency

One of the major lessons from this analysis is that a product can contribute significantly to sales while still creating substantial operational losses.

---

#  Strategic Recommendations

 1. Optimize Production Planning for High-Waste ProductsProducts such as **Sandwiches, Panipuri, and Sugarcane Juice** recorded the highest waste percentages.

 2. Waste concentration during specific periods suggests that preparation may occur before demand materializes.
 Historical sales patterns should be used to develop time-based production.

 3. Strengthen Inventory Monitoring

An overall waste rate of approximately **11%** represents a meaningful operational cost.
Regular inventory monitoring and product-level waste thresholds should be established to strengthen inventory monitoring.

 4. Reassess Underperforming High-Waste Menu Items

Products generating relatively high waste while contributing less to sales can negatively affect profitability.

 5. Establish Waste Performance KPIs

Waste reduction should be continuously monitored rather than treated as a one-time project.

 6. Integrate Sales and Inventory Reporting

The analysis demonstrates the value of looking at sales and waste together.

# Expected Business Impact

If the recommendations are implemented effectively, the business could potentially achieve:

* Lower food waste
* Reduced operational costs
* Better inventory utilization
* More efficient production planning
* Improved profit margins
* Better menu decisions
* Stronger operational accountability
* More evidence-based decision-making

---

# Project Limitations

The most important limitation is that the original sales dataset did not contain actual inventory and waste records.

Therefore, the inventory and waste component of this project is **simulated**.

The analysis demonstrates the **methodology and potential business intelligence solution**, but the waste-related findings should not be interpreted as actual historical performance from Balaji Restaurant.

---

# Future Improvements

With access to additional business data, this project could be extended into a more advanced restaurant analytics solution.

1. Customer Analysis
2. Basket Analysis
3. Ingredient-Level Waste Analysis
4. Forecasting
5. Profitability Analysis

---

# Tools Used

* **Power BI** — Data modelling, analysis and dashboard development
* **Power Query** — Data cleaning and transformation
* **DAX** — Calculated measures and analytical KPIs
* **Microsoft Excel** — Data preparation and supporting analysis

---

# Skills Demonstrated

* Data Cleaning
* Data Transformation
* Data Modelling
* DAX
* Power Query
* KPI Development
* Exploratory Data Analysis
* Time-Series Analysis
* Inventory Analytics
* Sales Analytics
* Restaurant Performance Analysis
* Dashboard Design
* Business Intelligence
* Data Storytelling
* Business Recommendation

---

# Project Outcome

This project demonstrates how combining **sales and inventory data** can reveal operational inefficiencies that traditional sales reporting may overlook.

Rather than focusing exclusively on revenue, the analysis connects **sales performance, production, waste, time, and profitability** to provide a more complete picture of restaurant operations.

The project ultimately demonstrates how business intelligence can turn operational records into actionable insights that support:

> **Better production decisions → Lower waste → Improved efficiency → Stronger profitability**

---

## About the Analyst

**Ariyibi Aminat**
Data & Business Intelligence Analyst

I use data analysis and business intelligence to help businesses turn everyday records into **clarity, insight, structure, and growth**.

**Tools:** Excel • SQL • Power BI • Python
**Focus:** Business Intelligence • Hospitality Analytics • Data-Driven Decision Making
