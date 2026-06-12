# Phone-Pe-Analysis
A comprehensive data analysis of PhonePe transactions, focusing on success rates, failure patterns, and transactional trends across different regions and time periods.

# PhonePe Pulse: End-to-End Transaction Status Analysis

## 📌 Project Overview
This project delivers a comprehensive data analysis of the PhonePe transaction ecosystem. The core objective is to evaluate transaction dynamics across India, with a dedicated focus on tracking **Transaction Statuses (Successful vs. Failed)**. By analyzing transaction failure rates, volumes, and values across different states, quarters, and payment categories, this project uncovers critical operational insights regarding digital payment success trends and regional infrastructure performance.

---

## 🛠️ Tech Stack & Tools Used
*   **Data Cleaning & Preprocessing:** Microsoft Excel (Power Query)
*   **Data Modeling & Visualization:** Power BI Desktop
*   **Analytical Calculations:** Advanced DAX (Data Analysis Expressions)

---

## 🚀 Key Features & Analytics Focus
*   **Success vs. Failure Deep-Dive:** Interactive KPI cards and charts isolating transaction success rates and visualizing failure patterns.
*   **Geographical Analysis:** Regional tracking across Indian states to identify areas experiencing higher transaction drops or peak performance.
*   **Temporal Trends:** Timeline analysis demonstrating how volumes and success ratios fluctuate quarter-on-quarter.
*   **Payment Type Performance:** Breakdown of success metrics by categories (Peer-to-peer, Merchant payments, Recharge & bill bills, etc.).

---

## 📈 Data Pipeline Architecture

### 1. Excel (Data Preparation)
*   Imported raw transaction status datasets.
*   Cleaned missing parameters, handled null values, and standardized naming conventions for Indian states and union territories.
*   Structured the metrics into highly optimized transactional flat tables.

### 2. Power BI Data Modeling
*   Established a robust Star Schema data model separating Fact tables (Transactions) from Dimension tables (Geography, Calendar/Time).
*   Configured relationships to enable seamless cross-filtering and drill-down functionality.

### 3. DAX Calculations
Implemented complex custom metrics using DAX to drive dynamic visual calculations. Key metrics include:
*   **Total Transactions:** `Total Transactions = COUNT(Transactions[Transaction_ID])`
*   **Successful Volume:** `Successful Transactions = CALCULATE(COUNT(Transactions[Transaction_ID]), Transactions[Status] = "Success")`
*   **Transaction Success Rate (%):** `Success Rate = DIVIDE([Successful Transactions], [Total Transactions], 0)`
*   *`[Add any other notable DAX formulas you created here, like YOY Growth or Failure Rates]`*


### Key Insights Uncovered:
*   **State Performance
*   **Success Ratios
