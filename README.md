# 🍽️ Restaurant Sales & Waste Reduction Analysis

## 📌 Project Overview

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

# 🎯 Business Problem

Restaurants can experience significant losses through:

* Overproduction
* Poor inventory planning
* Excessive food waste
* Inefficient production schedules
* Poor-performing menu items
* Misalignment between production volume and customer demand

Traditional sales reporting may identify which products generate the most revenue, but it does not necessarily explain whether those products are being produced efficiently.

### Business Question

> **How can sales and inventory waste data be combined to identify operational inefficiencies and opportunities to reduce waste while protecting profitability?**

---

# 🎯 Project Objectives

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

# 📊 Dataset

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

> **Important:** Inventory and waste figures in this project are simulated and should not be interpreted as actual operational records from the restaurant.

---

# 🔄 Methodology

The project followed a structured data analytics workflow from raw data preparation through business recommendations.

## 1. Data Collection

The restaurant sales dataset was obtained from Kaggle and examined to understand its structure, available fields, and suitability for the business questions.

Because inventory data was unavailable, a separate simulated waste dataset was developed to complement the sales information.

---

## 2. Data Cleaning & Preprocessing

The datasets were prepared for analysis using Power Query and Excel.

The cleaning process included:

* Removing duplicate records
* Standardizing product names
* Correcting date formatting
* Checking for missing values
* Resolving inconsistent text formatting
* Ensuring fields were stored using appropriate data types

The goal was to create consistent datasets that could be reliably connected during the modelling stage.

---

## 3. Data Transformation

Additional analytical fields were created to support the business questions.

Key calculated fields included:

* **Total Waste Cost**
* **Waste Percentage**
* **Total Margin**
* **Quantity Wasted**

These transformations allowed the analysis to move beyond basic sales reporting and evaluate operational efficiency.

---

## 4. Data Modelling

The Power BI model was structured around the relationship between sales, time, products, and inventory/waste.

### Model Structure

```text
             Calendar
                │
                │
                ▼
             Sales
                │
                │
          Product / Date
                │
                ▼
        Inventory / Waste
```

Relationships were established using:

* Date
* Product Name

This allowed sales and waste information to interact through Power BI's cross-filtering capabilities.

---

## 5. KPI Development

Executive-level KPIs were developed to provide an immediate overview of business performance.

The dashboard tracks:

* **Total Sales**
* **Total Margin**
* **Total Waste Cost**
* **Overall Waste Percentage**

These KPIs allow management to monitor financial performance and operational waste from a single view.

---

## 6. Exploratory Analysis

The analysis examined performance from several perspectives.

### Product Analysis

Products were evaluated based on:

* Revenue
* Quantity Sold
* Quantity Wasted
* Waste Cost
* Waste Percentage
* Margin

This helped identify products that were strong revenue generators, as well as products where waste was disproportionately high relative to sales.

### Time Analysis

Waste was analyzed by time of day to identify periods where production may not be aligned with customer demand.

### Sales vs Waste Analysis

Sales volume was compared against quantity wasted to identify potential overproduction and products requiring operational review.

---

## 7. Dashboard Development

The final Power BI dashboard was designed around several analytical components.

### Executive KPI Cards

Provides an immediate snapshot of:

* Total Sales
* Total Margin
* Total Waste Cost
* Overall Waste Percentage

### Sales & Waste Cost by Product

Compares product revenue against waste cost.

**Purpose:** Identify products generating revenue while simultaneously creating significant operational losses.

### Waste Cost by Time of Day

Shows when waste is concentrated throughout the operating day.

**Purpose:** Support better production scheduling and operational planning.

### Top 3 Products

Highlights the restaurant's strongest sales contributors.

**Purpose:** Identify core revenue-driving products.

### Quantity Sold vs Quantity Wasted

Compares customer demand against inventory loss.

**Purpose:** Identify potential overproduction.

### Underperforming High-Waste Products

Highlights products with relatively high waste and weaker sales.

**Purpose:** Support menu engineering and product-level decision-making.

### Waste Distribution Table

Provides a product-level comparison of waste percentages.

**Purpose:** Allow management to quickly identify products requiring attention.

---

# 📈 Key Performance Results

The dashboard revealed the following overall performance:

| KPI                          | Result |
| ---------------------------- | -----: |
| **Total Sales**              | ~$275K |
| **Total Margin**             | ~$161K |
| **Total Waste Cost**         |  >$14K |
| **Overall Waste Percentage** |   ~11% |

These figures highlight an important operational issue: even with strong sales and margin performance, waste represents a significant cost that can reduce the business's overall efficiency.

---

# 🔍 Key Insights

## 1. Waste Is Concentrated Among Certain Products

Several products contribute disproportionately to waste costs despite only moderate sales performance.

This suggests that sales volume alone should not determine production quantities.

These products require further investigation into:

* Batch sizes
* Ingredient purchasing
* Demand forecasting
* Production frequency

---

## 2. Waste Is Higher During Earlier Operating Hours

The time-of-day analysis showed that waste was highest during earlier operating periods before gradually declining throughout the day.

This pattern may indicate that some food is being prepared before sufficient customer demand has materialized.

> **Business implication:** Production schedules may need to be better aligned with expected demand throughout the day.

---

## 3. Some Products Show a Production–Demand Mismatch

Certain products showed a combination of:

* High production
* Lower sales
* Higher waste percentages

This represents a potential overproduction problem and an opportunity to improve inventory utilization.

---

## 4. High Sales Does Not Automatically Mean High Efficiency

One of the major lessons from this analysis is that a product can contribute significantly to sales while still creating substantial operational losses.

Therefore, restaurant performance should not be evaluated using revenue alone.

A more complete view should consider:

**Sales + Margin + Waste + Demand**

---

# 💡 Strategic Recommendations

## 1. Optimize Production Planning for High-Waste Products

Products such as **Sandwiches, Panipuri, and Sugarcane Juice** recorded the highest waste percentages.

### Recommendation

Implement demand-based production by:

* Preparing smaller initial batches
* Monitoring demand throughout the day
* Replenishing based on actual sales
* Adjusting preparation quantities based on historical patterns

This can reduce unnecessary waste while maintaining product availability.

---

## 2. Align Food Preparation With Customer Demand

Waste concentration during specific periods suggests that preparation may occur before demand materializes.

### Recommendation

Use historical sales patterns to develop time-based production schedules.

For example:

```text
Historical Demand
       ↓
Expected Customer Traffic
       ↓
Production Target
       ↓
Monitor Actual Sales
       ↓
Adjust Next Batch
```

This creates a more responsive production system instead of relying entirely on fixed preparation quantities.

---

## 3. Strengthen Inventory Monitoring

An overall waste rate of approximately **11%** represents a meaningful operational cost.

### Recommendation

Establish regular inventory monitoring and product-level waste thresholds.

Management could track:

* Waste Percentage
* Waste Cost
* Inventory Turnover
* Gross Margin
* Quantity Produced vs Sold

Products exceeding their waste thresholds should trigger further investigation.

---

## 4. Reassess Underperforming High-Waste Menu Items

Products generating relatively high waste while contributing less to sales can negatively affect profitability.

### Recommendation

Conduct periodic menu performance reviews to determine whether these products should receive:

* Recipe adjustments
* Portion adjustments
* Pricing changes
* Promotional support
* Production reductions
* Menu removal

---

## 5. Establish Waste Performance KPIs

Waste reduction should be continuously monitored rather than treated as a one-time project.

Recommended KPIs include:

* Waste Percentage
* Waste Cost
* Inventory Turnover
* Gross Margin
* Quantity Wasted
* Production-to-Sales Ratio

---

## 6. Integrate Sales and Inventory Reporting

The analysis demonstrates the value of looking at sales and waste together.

### Recommendation

Establish a recurring reporting process where management reviews:

**Sales → Inventory → Waste → Margin**

together rather than analyzing each independently.

This can support better decisions around:

* Purchasing
* Food preparation
* Staffing
* Inventory management
* Menu planning

---

# 📌 Expected Business Impact

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

# ⚠️ Project Limitations

The most important limitation is that the original sales dataset did not contain actual inventory and waste records.

Therefore, the inventory and waste component of this project is **simulated**.

The analysis demonstrates the **methodology and potential business intelligence solution**, but the waste-related findings should not be interpreted as actual historical performance from Balaji Restaurant.

In a real-world implementation, the model should be connected to:

* Actual inventory records
* Purchase records
* Ingredient usage
* Production records
* Waste logs
* Recipe/ingredient costs
* Customer feedback

This would enable more accurate operational and profitability analysis.

---

# 🚀 Future Improvements

With access to additional business data, this project could be extended into a more advanced restaurant analytics solution.

### Customer Analysis

Analyze:

* Customer frequency
* Customer lifetime value
* Customer preferences
* Repeat purchasing behavior

### Basket Analysis

Identify products frequently purchased together to support:

* Menu bundling
* Cross-selling
* Promotional offers

### Ingredient-Level Waste Analysis

Move from menu-item waste to ingredient-level analysis to identify the actual sources of food loss.

### Forecasting

Develop demand forecasts to estimate expected sales and determine optimal production quantities.

### Profitability Analysis

Combine ingredient-level costs with sales and waste to calculate more accurate product-level profitability.

---

# 🛠️ Tools Used

* **Power BI** — Data modelling, analysis and dashboard development
* **Power Query** — Data cleaning and transformation
* **DAX** — Calculated measures and analytical KPIs
* **Microsoft Excel** — Data preparation and supporting analysis

---

# 🧠 Skills Demonstrated

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

# 🎯 Project Outcome

This project demonstrates how combining **sales and inventory data** can reveal operational inefficiencies that traditional sales reporting may overlook.

Rather than focusing exclusively on revenue, the analysis connects **sales performance, production, waste, time, and profitability** to provide a more complete picture of restaurant operations.

The project ultimately demonstrates how business intelligence can turn operational records into actionable insights that support:

> **Better production decisions → Lower waste → Improved efficiency → Stronger profitability**

---

## 👩🏽‍💻 About the Analyst

**Aminat Amope**
Data & Business Intelligence Analyst

I use data analysis and business intelligence to help businesses turn everyday records into **clarity, insight, structure, and growth**.

**Tools:** Excel • SQL • Power BI • Python
**Focus:** Business Intelligence • Hospitality Analytics • Small Business Analytics • Data-Driven Decision Making
