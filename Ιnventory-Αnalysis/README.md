# 📦 Case Study: Inventory Analysis

> **Stakeholder:** Management Team at WarmeHands (Datacamp)  
> **Objective:** Optimize inventory control by classifying high-value items and identifying high-turnover products to reduce storage expenses and increase profitability.

## Project Overview
In this role as a Strategic Consultant for **WarmeHands Inc.**, I conducted a deep-dive inventory audit to solve a classic business problem: *Which items are worth the investment for restocking?* Using a fictitious dataset of 104 items across five categories, I moved from basic profit metrics to advanced efficiency ratios and classification models to provide data-driven purchasing recommendations.

## Dashboard Walkthrough
![Media/walkthrough_inv.gif](Media/walkthrough_inv.gif)

## Motivation & Problem Statement
Poor inventory management leads to high storage costs, capital tied up in "dead stock," and missed revenue from stockouts of popular items.
  * **The Challenge:** High sales volume doesn't always mean high efficiency. For example, some items sell in bulk but rotate slowly, while others sell quickly but at lower margins.
  * **The Goal:** Build a decision-support tool to:
      * Categorize inventory into **ABC classes** based on revenue contribution.
      * Measure **Inventory Turnover** to see how often stock is replaced.
      * Compare Year-over-Year (2020 vs. 2021) performance to identify growth trends.

## Technology & Process
  * **Tool:** Power BI.
  * **Dataset:** Six tables (SKU-ID, Orders, Initial Stock, Pricing, etc.) connected via a relational model.
  * **The Process:**
    1.  **Data Cleaning:** Structured SKU IDs, handled duplicates, and validated pricing and order dates.
    2.  **Financial DAX:** Created measures for **Revenue**, **COGS** (raw materials + labor), and **Gross Profit**.
    3.  **Efficiency Modeling:** Calculated **Average Inventory Value** and **Inventory Turnover Ratio** (COGS / Average Inventory).
    4.  **ABC Analysis:** Implemented a 4-step classification logic:
          * **A (Top 70%):** Critical items driving the bulk of revenue.
          * **B (Next 20%):** Mid-tier items.
          * **C (Final 10%):** Low-value or slow-moving items.

## Key Insights (Business Questions Answered)
  * **Volume vs. Velocity:** While "Grow a flytrap" has the highest total sales volume, "Doughnut lip gloss" has a superior **Inventory Turnover**, meaning it sells faster and frees up cash more efficiently.
  * **Growth Identification:** The "Set of 6 soldier skittles" was identified as the top-growing product between 2020 and 2021.
  * **Profit Concentration:** The Home and Accessories categories were identified as the primary profit drivers, reaching $110,000 in 2020 alone.
  * **Prioritization:** The ABC analysis confirmed that a small group of "Class A" items covers 70% of total revenue, allowing management to focus their strictest control policies on these specific SKUs.

## Challenges & Limitations
  * **Supply Chain Scope:** COGS calculations exclude transportation and distribution costs, meaning the "Net Profit" may be lower than the "Gross Profit" shown.
  * **Seasonality:** While Average Inventory accounts for some fluctuation, the model does not currently predict specific seasonal peaks (e.g., holiday spikes) for 2022.

## Repository Contents
  * `/Backgrounds`: Custom layouts for the WarmeHands inventory dashboard.
  * `/Dataset`: Six CSV files (Sales, Product, Stock, etc.).
  * `/Media`: Video walkthrough demonstrating the ABC classification and year-over-year slicers.
  * `/Template`: The Power BI template (.pbit) file.
  * `WarmeHands-Inventory-Optimization.pbix`: The final interactive report.
