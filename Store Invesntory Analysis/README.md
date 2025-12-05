# 📦 Inventory Data Analysis & Database Migration Project

This project demonstrates an end-to-end Business Intelligence solution for **Inventory Data Analysis** built in Power BI, showcasing advanced data modeling, DAX proficiency, and critical data engineering adaptability during a database migration.

The core objective was to track and visualize key supply-chain metrics across testing and production phases, while managing a live migration from MS SQL to MySQL.

## 🌟 Key Features & Problem Solved

This dashboard successfully addresses several real-world challenges:

1. **Dual-Phase Reporting:** The dashboard was first validated using **Test Data** during the system's pilot phase and later seamlessly transitioned to reflect **Production Data** without requiring visual redesign.

2. **Database Migration Replication:** The Power Query and data source setup was engineered to handle a critical enterprise change: migrating the backend from **MS SQL Server** to **MySQL**. This demonstrates flexibility in data connectivity and minimizing report downtime.

3. **Advanced KPI Calculation:** All core metrics are calculated using sophisticated DAX formulas to ensure accuracy regardless of the underlying data source.

## 📊 Dashboard Visuals & KPIs

The report is divided into two phases to showcase the transition from testing to a live environment. The primary focus is on inventory health, profitability, and operational stability.

### Key Performance Indicators (KPIs)

The following metrics were calculated using DAX to provide actionable insights:

| KPI Group | Specific Metrics | Purpose | 
 | ----- | ----- | ----- | 
| **Inventory Health** | `Average Demand per Day`, `Average Availability Per Day`, `Total Supply Shortage` | Measures the balance between stock and customer needs. | 
| **Financial** | `Total Profit`, `Total Loss`, `Average Daily Loss` | Assesses the financial impact of demand-availability mismatches. | 
| **Trends** | `Average Demand and Availability Trend` | Visualizes weekly/monthly volatility and seasonality in supply chain performance. | 

## 🖼️ Phase I: Pre-Production Dashboard (Test Data)

This view reflects the state of the report connected to the initial testing database (MS SQL), using simulated or scaled-down data to validate the model and DAX logic.

| **KPI Snapshot (Test Data)** | **Financial Snapshot (Test Data)** | 
 | ----- | ----- | 
| ![Inventory KPIs using Test Data](./images/test_kpis.png) | ![Financial KPIs using Test Data](./images/test_financials.png) | 

**Key Insight:** *Notice the distinct values that confirm the test environment is running successfully and the DAX measures are calculating correctly before going live.*

## 🖼️ Phase II: Post-Production Dashboard (Live Data)

This view demonstrates the same report visuals and DAX logic but connected to the live **Production Data** after the database migration to **MySQL** was successfully completed.

| **KPI Snapshot (Live Data)** | **Financial Snapshot (Live Data)** | 
 | ----- | ----- | 
| ![Inventory KPIs using Live Data](./images/prod_kpis.png) | ![Financial KPIs using Live Data](./images/prod_financials.png) | 

**Key Insight:** *The updated, larger values confirm the data sources were successfully swapped and the migration was seamless, validating the stability of the Power Query setup.*

### Trend Analysis (Applicable to Both Phases)

This chart shows the historical trend of demand versus availability over time, which is critical for forecasting and identifying operational bottlenecks.

![Demand and Availability Trend](./images/trend_analysis.png)

## 🛠️ Technical Details & Setup

* **Software:** Power BI Desktop

* **Initial Data Source:** Microsoft SQL Server

* **Final Data Source:** MySQL

* **Modeling:** Star Schema optimized for inventory transactions.

* **Data Transformation:** Power Query used for dynamic source switching and detailed cleaning of date and product fields.

## ➡️ Accessing the Project

1. **Required:** Power BI Desktop (Latest Version)

2. **Files:** The primary Power BI file is located at `[FILEPATH_TO_PBIX_OR_PBIP_FILE]`. *(Replace with the path to your main Power BI file)*

3. **Data Source Link:** The external raw data source is available at: `[LINK_TO_YOUR_DATA_SOURCE_OR_NOTE]` *(Replace with a link or note about the data location)*
