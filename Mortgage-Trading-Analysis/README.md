# 📉 Case Study: Mortgage Trading Analysis

> **Stakeholder:** Sooper Mortgage (Datacamp)         
> **Objective:** Execute a strategic trade of 5,000+ mortgages by identifying the optimal loan population and evaluating competitive bids to maximize trade revenue.

## Project Overview
In this advanced case study, I acted as a **Junior Trader** for a mortgage originator. The project simulates the lifecycle of a mortgage within the broader financial system—from lending to borrowers to selling those loan agreements to large investment banks. I was responsible for data modeling the loan population, calculating the current principal via amortization, and executing a trade that balances firm profitability with market competitiveness.

## Financial Report Walkthrough
![Media/walkthrough_mor.gif](Media/walkthrough_mor.gif)

## Motivation & Problem Statement
Lenders must sell their loans in the capital markets to regain the liquidity needed to issue new loans. This "recycling" of money is the heartbeat of the financial system.
  * **The Challenge:** Determining which loans to sell and at what price requires balancing risk (Credit Scores, LTV) against market demand.
  * **The Goal:** To build a trading desk financial report that allows the desk to:
      * Filter and identify a trade-ready population of mortgages.
      * Compare bids from multiple institutional buyers to find the **Maximum Bid**.
      * Analyze the **Weighted Average Price** to understand the true value of the trade.

## Technology & Process
  * **Tool:** Power BI.
  * **Advanced Techniques:** Power Query (M), Financial DAX, and AI Analytics.
  * **The Process:**
    1.  **Data Transformation:** Used Power Query to clean disparate datasets and applied **M code** to create a "Winner Takes All" logic to identify the best bidder for each loan.
    2.  **Amortization Modeling:** Developed DAX measures using the `PPMT` function to calculate monthly principal payments and current loan balances.
    3.  **Risk Profiling:** Segmented the portfolio by **Loan-to-Value (LTV)** and **Debt-to-Income (DTI)** ratios to evaluate the risk-adjusted value of the assets.
    4.  **Trade Execution:** Built a cohesive data model that calculates trade premiums, revenue, and profit margins at the individual loan and portfolio levels.

## Key Insights (Business Questions Answered)
  * **Optimal Execution:** Identified which loans yielded the highest premiums when sold as Whole Loans versus those better suited for Mortgage-Backed Securities (MBS).
  * **Profit Drivers:** Used the **Key Influencers** AI visual to determine that interest rates and borrower credit scores were the strongest predictors of trade profitability.
  * **Market Position:** Analyzed the firm's "bid-to-cover" ratio to see if Sooper Mortgage was pricing its loans too aggressively, leading to lost business.
  * **Financial Flow:** Visualized how money moves from savers/investors through the trading desk to provide capital for home borrowers.

## Challenges & Limitations
  * **Static Pricing:** The model uses a fixed date (Sept 21, 2021); in a live environment, mortgage prices fluctuate daily based on Treasury yields.
  * **Prepayment Risk:** The analysis assumes loans pay as scheduled; in reality, borrowers often refinance or pay early, which complicates the "Future Value" of the trade.

## Repository Contents
  * `/Datasets`: Six Excel sheets.
  * `/Media`: A video walkthrough of the financial report.
  * `/Theme`: The Power BI theme for the financial report.
  * `Mortgage-Trading-Analysis.pbix`: The final interactive financial report.
