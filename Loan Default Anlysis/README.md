#  Loan Default Risk Analysis Dashboard (Power BI)

This project provides a comprehensive analysis of a loan portfolio to identify key risk factors contributing to loan defaults. It utilizes a robust Power BI architecture, including Dataflows for shared data preparation and advanced DAX measures for calculating key financial and risk metrics.

The primary goal is to empower the lending team with actionable insights to inform underwriting decisions, portfolio management, and strategy development.

##  Project Goal and Methodology

### Goal

* **Identify and quantify** the main drivers of loan default risk (e.g., Credit Score, DTI, Employment Type).
* **Establish a single source of truth** for key loan metrics using Power BI Dataflows.
* **Visualize portfolio health** through an interactive, multi-page dashboard.

### Methodology

1.  **Data Ingestion & Preparation:** Initial data is loaded and transformed using Power Query in a centralized Power BI **Dataflow** for shared data access across the team.
2.  **Data Modeling:** A clean data model is established within the Power BI Desktop file.
3.  **Advanced Calculations (DAX):** Measures like **Default Rate**, **Year-over-Year (YoY) Change**, and conditional aggregations are calculated using DAX formulas.
4.  **Visualization:** Data is presented across four specialized dashboard pages to serve different analytical needs.

##  Data Dictionary

The analysis is based on the following key variables from the Loan Default Dataset:

| Column Name | Description | Key Use in Dashboard |
| :--- | :--- | :--- |
| **LoanAmount** | Total loan amount. | Total Loan Amount KPI, Distribution Charts. |
| **CreditScore** | Borrower's creditworthiness (300-850). | Primary risk factor, used in **Default Rate by Credit Score** chart. |
| **DTIRatio** | Debt-to-Income ratio. | Financial burden analysis. |
| **LoanTerm** | Length of the loan in months. | Average Loan Term KPI. |
| **EmploymentType** | Borrower's job status (e.g., Full-Time, Self-Employed). | Used in **Default Rate by Employment type** chart. |
| **Education** | Highest level of education completed. | Used in **Loans by Education Type** chart. |
| **Default** | Indicator (Yes/No) if the loan defaulted. | Primary metric for calculating **Default Rate**. |
| **Loan Date** | Date the loan was issued. | Used for **Year-over-Year (YoY)** trend analysis. |

##  Dashboard Pages and Insights

The Power BI report is structured into four main pages to guide the user from high-level portfolio health to detailed risk factors.

### 1. Executive Summary & Key Risk Factors

<img width="1412" height="794" alt="Screenshot 2025-12-06 173707" src="https://github.com/user-attachments/assets/fa617064-6567-47a2-89c6-aaafbb43ad6c" />

* **KPIs:** Provides the immediate health check: **Total Loan Amount**, **Default Rate**, **Average CreditScore**, and **Average Loan Term**.
* **Trend Analysis:** The **Default Rate by Year** line chart shows the overall historical risk trend.

### 2. Loan Default and Overview

<img width="1412" height="794" alt="Screenshot 2025-12-06 173804" src="https://github.com/user-attachments/assets/94def7ee-69a0-449c-8332-e96ae0aa65a2" />

* **Key Insight:** Loans for **Business** purposes often account for a high total loan amount, requiring close monitoring.
* **Risk Gradient:** Default rate is highest for lower credit score bins and for **Unemployed** borrowers, highlighting clear risk segmentation.

### 3. Applicant Demographic and Financial Profile

<img width="1412" height="794" alt="Screenshot 2025-12-06 173820" src="https://github.com/user-attachments/assets/3007cb24-0fae-4b25-bc27-8e2d552c0916" />

* **Demographic Volume:** Analyzes loan volume by **Education Level** and **Marital Status**.
* **Credit Distribution:** Visualizes the median and total loan amount across different credit score and age bins.

### 4. Financial Risk Matrix

<img width="1412" height="794" alt="Screenshot 2025-12-06 173835" src="https://github.com/user-attachments/assets/01a5cab3-0e51-4f12-acc3-f5d5b38bea5c" />

* **Year-over-Year (YoY) Tracking:** This chart compares the annual percentage change of a key metric (e.g., Loan Volume) with the annual percentage change in default loans. This helps identify if periods of high growth correspond with changes in default risk.

##  Installation and Usage

1.  **Power BI Access:** Ensure you have access to the Power BI Service where the Dataflow is published.
2.  **Clone Repository:** Download or clone this repository to your local machine.
3.  **Open Report:** Open the provided `.pbix` file in Power BI Desktop.
4.  Source file is also attached in the same folder.

