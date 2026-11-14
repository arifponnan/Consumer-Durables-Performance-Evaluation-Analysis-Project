# Consumer Durables Executive Performance Dashboard (2022–2024)

## Executive Summary

This project delivers a consolidated **Executive Performance Dashboard** for a pan-India Consumer Durables company operating across **8 product categories**, **5 distribution channels**, and **80+ dealer partners**. By integrating three years (2022–2024) of monthly SKU sales (7,200+ rows), warehouse inventory logs, dealer credit ledgers, and multi-category marketing budgets, this solution provides senior leadership with a unified reporting layer for **Quarterly Business Reviews (QBRs)**.

The analysis uncovers critical revenue recovery opportunities in **Andhra Pradesh (-32% YoY)**, flags **17 credit-risk dealer partners**, isolates high-return SKUs eroding profitability (**AC-1.5T-WS**), and resolves supply chain imbalances across **Mumbai** and **Chennai** regional warehouses.

---

## Dashboard Preview & Screenshots

### 1. Executive Revenue, Seasonality & Mix Overview
*Tracks YoY revenue trends, gross margin performance, 3-year category/channel mix shifts, and multi-dimensional revenue and profit decomposition.*

<img width="1000" height="580" alt="image" src="https://github.com/user-attachments/assets/c6328e7c-f884-470b-af2d-b13213c8fbb8" />


### 2. Customer Quality & Dealer Network Health
*Highlights high-return/low-CSAT SKU outliers, regional service call heatmaps, and the high-risk dealers exceeding credit limits.*

<img width="1352" height="772" alt="image" src="https://github.com/user-attachments/assets/12784fbc-ebcf-4858-b4c1-aa60f94cba87" />


### 3. Marketing ROI & Inventory Risk Management
*Evaluates category wise Cost Per Lead (CPL), ad-spend-to-revenue correlation, warehouse stockout gaps in region and SKU , and excess stock exposure.*

<img width="1407" height="781" alt="image" src="https://github.com/user-attachments/assets/2676f316-0ae0-4908-94a4-e5c68e8bc61c" />


---

## Project Objective

The objective of this analysis is to build a consolidated performance dashboard that integrates commercial sales, warehouse inventory, dealer network health, and marketing efficiency data into a single source of truth to support executive decision-making during Quarterly Business Reviews.

### Core Business Questions Addressed

1. **Revenue & Profitability:** How is the business trending YoY, and which categories, regions, and channels drive the most revenue and gross margin?

2. **Seasonality & Mix:** Where are the seasonal spikes, and how has the product/channel mix shifted over 3 years?

3. **Customer Quality:** Which SKUs and segments have the highest return rates and lowest CSAT, and where are service calls concentrated?

4. **Dealer Health:** Which dealers are at risk (high outstanding balance vs. credit limit, paired with below-target achievement), and is there a regional concentration of underperformers?

5. **Marketing Efficiency:** What is the Cost Per Lead (CPL) by category, and does higher ad spend correlate with revenue growth?

6. **Inventory Risk:** Which SKUs are sitting below reorder levels, and where is overstock risk concentrated?

## Dataset Overview

The underlying data model connects five core tables covering 2022–2024 operations:

| Sheet / Table Name | Scope & Granularity | Key Metrics & Attributes | 
| ----- | ----- | ----- | 
| **`Sales_Data`** | 7,200 rows of monthly SKU sales | Revenue, COGS, Gross Profit, Returns, CSAT, and Service Calls by SKU, Region, Channel & Segment | 
| **`Inventory`** | SKU-level warehouse stock | Current Stock, Reorder Levels, Supplier Lead Times, and Warehouse Mapping | 
| **`Dealer_Network`** | 80+ authorized dealer partners | Sales Targets, YTD Achievement, Credit Exposure, and Net Promoter Score (NPS) | 
| **`Marketing_Spend`** | Monthly category media budgets | Spend breakdown across TV, Digital, Print, BTL, and Sponsorships | 
| **`Data_Dictionary`** | Schema metadata | Definitions and business rules for every column | 

## Analysis Approach & Visual Methodology

* **Seasonality & Portfolio Mix Shift:** Visualized 3-year demand trajectories using **Line and Stacked Area Charts** to identify seasonal spikes and structural shifts in the category and channel mix. Deployed a **Decomposition Tree** to drill down into multi-dimensional revenue and gross margin distribution across regions and segments.

* **Customer Quality & Dealer Network Health:** Constructed a quadrant **Scatter Plot** comparing **Return Ratio vs. Average CSAT** to isolate critical SKUs eroding profitability and brand perception. Utilized a **Geospatial Map Visual** to pinpoint regional concentrations of post-sales service calls, and built a partner risk framework evaluating **Credit Limit Utilization** against **YTD Target Achievement**.

* **Marketing Efficiency & ROI:** Analyzed category-level **Cost Per Lead (CPL)** and evaluated statistical correlation between multi-channel ad spend and top-line revenue growth.

* **Inventory & Supply Chain Optimization:** Calculated dynamic safety stock buffers based on supplier lead times to flag both stockout and overstock risks, quantifying exact **Reorder Gaps** and **Excess Stock Units** by warehouse and SKU.

## Key Analytical Findings

* **Regional Revenue Contraction:** **Andhra Pradesh** experienced a sharp **32% YoY decline in revenue**, driven primarily by a steep drop in **Television** category sales.

* **Product Quality Outliers:** Quadrant analysis revealed specific SKUs—most notably **AC-1.5T-WS**—suffering from the highest product return rates alongside the lowest average CSAT scores.

* **Dealer Credit Exposure:** **17 dealers** are operating in a critical risk zone where credit utilization exceeds **100% of their credit limit** while YTD sales achievement remains **below 75%** (High-priority accounts: **DL1079, DL1064, and DL1053**).

* **Marketing Spend Misalignment:** **Refrigeration** and **Vacuum Cleaners** exhibit a **negative correlation between ad spend and revenue**, signaling diminishing returns. Conversely, **Washing Machines** generate high revenue velocity paired with low-cost lead generation.

* **Critical Stockout Risk:** **13 SKUs** have fallen below safety reorder thresholds, creating a cumulative replenishment deficit of **288 units**. The **Mumbai Warehouse** faces the highest shortage, specifically in Vacuum Cleaners (**Model: VC-ROBOT-STD**).

* **Warehouse Overstock:** The **Chennai Warehouse** holds the highest concentration of excess inventory, highlighted by **29 surplus units** of model **REF-250L** *(Refrigeration / Cooling division)*.

## Strategic Recommendations

| Focus Area | Finding / Target Entity | Actionable Recommendation | Expected Business Impact | 
| ----- | ----- | ----- | ----- | 
| **Regional Recovery** | Andhra Pradesh (Television: -32% YoY) | Focus regional ad spend and localized promotional bundles on the Television category in Andhra Pradesh | Reverses regional volume contraction and recaptures lost category share | 
| **Product R&D & QA** | High-Return / Low-CSAT SKUs (AC-1.5T-WS) | Escalate flagged SKUs to the R&D and QA teams for engineering improvements and product viability studies | Reduces return erosion, lowers service call volume, and lifts regional CSAT | 
| **Credit Governance** | 17 Critical Dealers (DL1079, DL1064, DL1053) | Freeze credit extensions for dealers >100% credit limit and <75% target achievement; enforce collection milestones | Mitigates bad-debt exposure and improves working capital recovery | 
| **Marketing Reallocation** | Refrigeration & Vacuum Cleaners vs. Washing Machines | Audit inefficient ad spend in Refrigeration and Vacuum Cleaners; reallocate budget to low-CPL, high-revenue categories like Washing Machines | Optimizes blended ROAS and accelerates top-line revenue growth | 
| **Stockout Replenishment** | 13 Stockout SKUs (288-unit gap; Mumbai WH: VC-ROBOT-STD) | Expedite purchase orders to close the 288-unit reorder gap, prioritizing VC-ROBOT-STD shipments to Mumbai WH | Prevents imminent lost sales and stabilizes regional order fulfillment | 
| **Inventory Rebalancing** | Chennai WH Overstock (Model REF-250L: 29 excess units) | Execute inter-warehouse stock transfers from Chennai to high-demand hubs or bundle excess units with fast-moving SKUs | Unlocks trapped working capital and reduces warehouse holding costs | 
