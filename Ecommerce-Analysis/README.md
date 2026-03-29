# 🐶Case Study: Ecommerce Analysis

> **Stakeholder:** Whiskique Management Team (Datacamp).        
> **Objective:** Drive sales growth through upselling/cross-selling and reduce operational expenses by optimizing "last-mile" shipping costs.

## Project Overview
In this role as a Data Analyst for **Whiskique**, an online pet supply retailer, I transformed raw e-commerce data into a strategic tool for decision-making. The project focuses on the delicate balance between high-volume sales and the underlying costs of the supply chain—specifically COGS, freight, and last-mile delivery.

## Dashboard Walkthrough
![Media/walkthrough_ec.gif](Media/walkthrough_ec.gif)

## Motivation & Problem Statement
Whiskique faces the classic e-commerce challenge: growing the customer base while protecting profit margins from rising fulfillment costs.
  * **The Challenge:** Shipping costs (averaging $5 per unit in our canned food model) significantly eat into the $8 profit margin.
  * **The Goal:** Build an interactive Power BI suite to:
      * Identify **Upsell** (higher-priced alternatives) and **Cross-sell** (relevant add-ons) opportunities.
      * Perform **What-If Analysis** to visualize how increasing shipping quantities per order impacts the bottom line.
      * Map the relationship between Product, Customer, and State data to find regional efficiency gaps.

## Technology & Process
  * **Tool:** Power BI.
  * **Data Architecture:** Developed a relational model using four CSV sources (**Sales, Product, Customer, and State Mapping**) connected via a Star Schema.
  * **The Process:**
    1.  **Supply Chain Modeling:** Integrated cost structures (COGS, Freight, Fulfillment, and Shipping) into the data model to calculate true profit.
    2.  **What-If Parameters:** Created a dynamic "Average Shipped Quantity" parameter to simulate cost savings across the business.
    3.  **Market Basket Insights:** Analyzed product correlations to identify which items are frequently bought together to inform marketing strategies.
    4.  **UI/UX:** Focused on "Dashboard-style" pages using high-contrast KPIs for Sales and Shipping Savings to ensure immediate clarity for management.

## Key Insights (Business Questions Answered)
  * **Shipping Optimization:** Demonstrated that consolidating shipments or increasing the units-per-package directly reduces "last-mile" expenses, significantly increasing the net profit per transaction.
  * **Growth Levers:** Identified specific organic pet food lines that serve as high-value "Upsell" targets for customers currently buying standard recurring items.
  * **Inventory Correlation:** Highlighted product pairs that are regularly purchased together, providing a roadmap for point-of-purchase cross-sell offers.
  * **Financial Transparency:** Provided a clear view of the "Landed Cost" vs. "Retail Price," allowing management to see exactly where margins are being eroded.

## Challenges & Limitations
  * **Market Basket Complexity:** While high-frequency pairs were identified, full correlation coefficient analysis was out of scope due to the need for advanced nested DAX formulas.
  * **Fictitious Constraints:** As the data is synthetic, external market factors (competitor pricing, fuel surcharges) were not factored into the shipping cost model.

## Repository Contents
* `/Datasets`: The datasets.
* `/Media`: A video walthrough of the dashboard.
* `/Theme`: The theme of the dashboard.
* `Ecommerce-Analysis.pbix`: The final Power BI interactive dashboard.
