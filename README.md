# Insurance Policy & Claims Data Simulation

## Project Overview
This project simulates a large-scale insurance dataset to analyze policy sales, claims behavior, and profitability trends. The goal is to generate synthetic data representing vehicle insurance policies and claims activity over multiple years and use it to perform analytical queries.

The project demonstrates how structured datasets can be created using programmatic rules and distributions to mimic real-world business scenarios. It also shows how such datasets can be used to derive insights about revenue, claims costs, and overall portfolio performance.

---

## Problem Statement
Insurance companies need historical data to evaluate risk patterns, estimate liabilities, and analyze profitability across different policy types. However, real datasets are often unavailable due to privacy or regulatory restrictions.

This project addresses that problem by:

- Simulating **policy sales data** for a full year
- Generating **claims data based on predefined business rules**
- Enabling **analysis of premium revenue and claim costs**
- Supporting **risk and profitability analysis**

The generated dataset can be used for analytics, SQL practice, business intelligence dashboards, or data engineering workflows.

---

## Dataset Description

### Policy Sales Dataset

This dataset represents vehicle insurance policies purchased during a specific year.

**Fields**

| Column | Description |
|------|-------------|
| Customer_ID | Unique identifier for each customer |
| Vehicle_ID | Unique identifier for each vehicle |
| Vehicle_Value | Fixed vehicle value |
| Premium | Premium paid based on policy tenure |
| Policy_Purchase_Date | Date when the vehicle and policy were purchased |
| Policy_Start_Date | Policy activation date |
| Policy_End_Date | Policy expiry date |
| Policy_Tenure | Policy duration in years |

**Key Assumptions**

- Policies are distributed across all days of the year.
- Policy tenures follow a predefined distribution.
- Policy start date begins after a fixed waiting period.
- Premium amount is determined by policy duration.

---

### Claims Dataset

This dataset represents insurance claims filed after policy activation.

**Fields**

| Column | Description |
|------|-------------|
| Claim_ID | Unique identifier for each claim |
| Customer_ID | Customer who filed the claim |
| Vehicle_ID | Vehicle associated with the claim |
| Claim_Amount | Amount paid for the claim |
| Claim_Date | Date when the claim was filed |
| Claim_Type | Indicator for claim category |

**Key Assumptions**

- Only vehicles purchased on specific calendar days are eligible for claims during the first claim period.
- A percentage of eligible vehicles file claims.
- Claims occur when policies are active.
- Vehicles with long-term policies may file additional claims later.

---

## Objectives

The generated datasets allow analysis of several key metrics:

- Total premium revenue collected
- Monthly claim costs
- Claim-to-premium ratios
- Profitability by policy duration
- Estimated future claim liabilities
- Earned vs unearned premium calculations

These insights help evaluate risk exposure and financial performance.

---

## Technologies Used

- **Python**
- **Pandas**
- **NumPy**
- **SQL (for analytical queries)**
- **Data visualization tools (optional)**

---

## Project Structure
