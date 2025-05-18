# Loan Portfolio Dashboard

### Dashboard Link : https://app.powerbi.com/groups/c5c6dc90-c94a-4976-a473-05668be8bc11/reports/8415be34-8629-4ae1-b4c3-f2b9e7a437ce/a46131874bc135d4de0a?experience=power-bi
### Dataset Link : https://drive.google.com/file/d/1OyHBNoiY3XLMaVqaz5HN5c_HNYAOrn-z/view?usp=drive_link
## Business Context:

A mid-sized digital lending company offers personal loans to individuals across India. The company has been issuing loans since 2013 and has amassed over 200,000 loan records. They now want to monitor loan performance, borrower profiles, and credit risk using a comprehensive Power BI dashboard.

## Business Goals and Objectives
1.	Track overall loan performance: total disbursed amount, interest income, average loan size.
2.	Reduce default rate: identify high-risk borrower patterns by credit score, income, employment type, DTI ratio.
3.	Optimize customer acquisition: identify which demographics and loan purposes are most profitable.
4.	Support data-driven lending decisions: build borrower profiles that reduce risk while maximizing growth.
5.	Monitor portfolio growth and trends over time and across segments.

## Key Business Questions to Answer
📈 Portfolio Performance

•	How many loans have been issued over time?

•	What is the total and average loan amount disbursed?

•	What is the total interest revenue?


💸 Credit Risk

•	What is the overall default rate?

•	What are the default rates by credit score, income bracket, age group, or employment type?

•	Are co-signed loans less likely to default?

👥 Customer Profile Insights

•	What is the demographic profile (age, income, employment) of borrowers?

•	How does loan performance vary by loan purpose or marital status?

•	Are certain education or employment types riskier?



## Setup Instructions for Power BI Gateway Integration with SQL & Incremental Refresh


### 1. Prepare the SQL Database
- Ensure your SQL Server is accessible and has the required data views/tables.
- Use indexed datetime columns for incremental refresh logic.

### 2. Develop Power BI Report
- Load data from SQL Server using DirectQuery or Import mode.
- Apply filters using parameters like `RangeStart` and `RangeEnd` in Power Query.
- Define policies for incremental refresh in the Power BI model settings.

### 3. Configure On-Premises Gateway
- Install and register the [On-Premises Data Gateway](https://learn.microsoft.com/en-us/data-integration/gateway/service-gateway-install) on your server.
- Map your local SQL connection to the cloud Power BI service.

### 4. Publish & Schedule Refresh
- Publish the Power BI report to Power BI Service.
- Set up the data source credentials and schedule refresh via the gateway.
## 🔄 Incremental Refresh Logic

Ensure your table contains a **DateTime column** to be used for partitioning. Power BI uses `RangeStart` and `RangeEnd` parameters for dynamic filtering.


# Snapshot of Dashboard (Power BI Service)

### 🔵 1. Overview
- Total Borrowers: **255.35K**
- Avg. Interest Rate: **13.5%**
- Avg. Borrower Age: **43.5 years**
- Avg. Credit Score: **574**

#### Key Visuals:
- Loans distributed by **Year**, **Credit Lines**, and **Income Bracket**
- **Default Rate Trend** (Year-wise)
- **Loan Purpose** & **Marital Status by Age Group**

![image](https://github.com/user-attachments/assets/3ac45f7d-276d-4b31-ad23-db4191faa08a)

### 🔴 2. Risk Evaluation & Default Patterns
- Total Defaults: **29.65K**
- Avg. Defaulter Income: **71.84K**
- Avg. DTI Ratio: **0.50**
- Avg. Credit Score (Defaulters): **559.29**

#### Key Visuals:
- **Loan Defaults by Year, Employment Type, and Purpose**
- Credit Score vs. Default Frequency
- Default Rates across **Income Brackets**, **Age Groups**, and **Loan Purposes**

![image](https://github.com/user-attachments/assets/0224a86b-b1e5-484c-a26a-934985e6bd64)

### 🔵 3. Business Performance Analysis
- Total Loan Amount: **₹32.6 Billion**
- Total Interest Income: **₹439.28 Billion**
- Avg. Credit Score (Non-defaulters): **576**
- Avg. Loan Term: **36.03 months**

#### Key Visuals:
- Loan Amount & Interest Income trends (by year)
- Loan Distribution by **Credit Score**, **Employment Type**, and **Income Bracket**

![image](https://github.com/user-attachments/assets/00a18dc7-8207-49f5-b0de-0dcd8378b1c7)

#### Key Visuals:
- Interest Income by **Credit Score**, **Employment Type**, and **Income Bracket**

![image](https://github.com/user-attachments/assets/809664d3-faf6-46b4-91af-1486bfb61b6e)

## 🛠️ Tools & Technologies Used

| Tool      | Purpose                              |
|-----------|--------------------------------------|
| **Power BI** | Data visualization & dashboard creation |
| **Excel / CSV** | Data transformation, cleaning |
| **DAX** | Calculated columns, measures |



## 🚀 Key Insights

- **High-income groups** account for a majority of the loan disbursal and defaults.
- **Unemployed and self-employed individuals** show higher default rates.
- Most defaults come from **medium to high credit score groups**, indicating more than just credit score affects risk.
- **Business and education loans** have higher default risks.
- Interest income peaked in **2015 and 2018**, aligned with peak loan issuance.


