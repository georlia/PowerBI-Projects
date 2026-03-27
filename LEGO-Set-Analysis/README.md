# 🧱 LEGO Set Explorer  

> **Stakeholder:** Maven Analytics.  
> **Objective:** Develop an interactive catalog to analyze LEGO set distribution, pricing trends, and part counts across various themes.

## Project Overview
In this project, I built a comprehensive Power BI report to explore a dataset of LEGO sets. The analysis focuses on providing a user-friendly interface to navigate thousands of products, filtering by theme groups, age ranges, and price points to help collectors or analysts identify specific market segments.

## Dashboard Walkthrough
![Media/walkthrough.gif](Media/walkthrough.gif)

## Motivation & Problem Statement
With thousands of LEGO sets released over decades, navigating the inventory to find specific value-for-money metrics or age-appropriate sets can be overwhelming.
  * **The Challenge:** Raw LEGO data contains noise (missing prices/URLs) and requires logical grouping to be useful for consumer analysis.
  * **The Goal:** To create a dynamic dashboard that allows users to:
      * Quickly filter sets based on specific price thresholds and age categories.
      * Visualize individual set details (images and specs) through interactive table hovers.
      * Analyze the hierarchy of LEGO products from broad categories down to individual set names.

## Technology & Process
  * **Tool:** Power BI
  * **Dataset:** LEGO sets CSV containing set IDs, themes, piece counts, and pricing.
  * **The Process:**
    1.  **Data Cleaning & Profiling:** Removed unnecessary fields (minifigs, URLs), handled missing values for price and age, and validated data types.
    2.  **Feature Engineering:** Created conditional columns for **Age Range** (e.g., "Over 18", "10 to 17") and **Price Range** (symbolic "$" to "$$$$$" ratings).
    3.  **DAX Measures:** Developed measures for Total Sets, Total Groups, Average Age, and Average Pieces.
    4.  **Advanced Interactivity:** Implemented a **Numeric Range Parameter** for dynamic price filtering and **Report Page Tooltips** to display set images on hover.

## Key Insights (Business Questions Answered)
  * **Inventory Distribution:** Identified which theme groups (e.g., Star Wars, Technic) command the highest average piece counts versus those with the highest average prices.
  * **Pricing Tiers:** Segmented the catalog to show the volume of "Budget" ($) vs. "Premium" ($$$$$) sets available.
  * **Hierarchical Analysis:** Used a **Decomposition Tree** to break down the total set count by category, theme group, and theme, revealing the most "crowded" segments of the LEGO catalog.

## Challenges & Limitations
  * **Data Completeness:** Several records were filtered out due to missing price or piece count data, which may slightly skew the "Average Price" for older, retired sets.
  * **Visual Performance:** Managing high-resolution image tooltips for a large table required optimization to ensure smooth hovering and selection.

## Repository Contents
  * `/Datasets`: The LEGO sets CSV dataset.
  * `/Media`: A video walkthrough of the dashboard.
  * `LEGO-Set-Explorer.pbix`: The final Power BI interactive dashboard.
  * `Lego_Logo.png`: A logo of LEGO company.
