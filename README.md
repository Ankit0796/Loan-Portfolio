# 📊 Loan Portfolio Insights Dashboard (2013–2018)

## 🧾 Overview

This project is a comprehensive Power BI dashboard built to analyze a loan portfolio dataset spanning from **2013 to 2018**. It is divided into three key segments:

1. **Portfolio Overview**
2. **Risk Evaluation & Default Patterns**
3. **Business Performance Analysis**

The dashboard enables stakeholders to monitor borrower behavior, identify high-risk areas, and analyze business performance over time.

---

## 📁 Dataset Features

The dataset consists of detailed loan information with the following columns:

| Column Name         | Description |
|---------------------|-------------|
| `LoanID`            | Unique identifier for each loan |
| `Age`               | Age of the borrower |
| `Income`            | Annual income of the borrower |
| `LoanAmount`        | Total loan amount |
| `CreditScore`       | Borrower's credit score |
| `MonthsEmployed`    | Duration of employment in months |
| `NumCreditLines`    | Number of active credit lines |
| `InterestRate`      | Interest rate on the loan |
| `LoanTerm`          | Duration of the loan in months |
| `DTIRatio`          | Debt-to-Income Ratio |
| `Education`         | Education level of the borrower |
| `EmploymentType`    | Employment status (e.g., Full-time, Part-time) |
| `MaritalStatus`     | Marital status (Single, Married, Divorced) |
| `HasMortgage`       | Binary flag indicating if the borrower has an existing mortgage |
| `HasDependents`     | Binary flag for number of dependents |
| `LoanPurpose`       | Purpose of the loan (Home, Auto, Education, etc.) |
| `HasCoSigner`       | Whether a co-signer is present |
| `Default`           | Binary flag indicating loan default |
| `Date`              | Date of loan origination |
| `CreditScoreBin`    | Categorized credit score (Very Low to High) |
| `IncomeBracket`     | Categorized income levels (Low, Medium, High) |
| `AgeBracket`        | Grouped age categories (Teen, Adult, etc.) |

---

## 📌 Dashboard Highlights

### 🔵 1. Overview
- Total Borrowers: **255.35K**
- Avg. Interest Rate: **13.5%**
- Avg. Borrower Age: **43.5 years**
- Avg. Credit Score: **574**

#### Key Visuals:
- Loans distributed by **Year**, **Credit Lines**, and **Income Bracket**
- **Default Rate Trend** (Year-wise)
- **Loan Purpose** & **Marital Status by Age Group**

---

### 🔴 2. Risk Evaluation & Default Patterns
- Total Defaults: **29.65K**
- Avg. Defaulter Income: **71.84K**
- Avg. DTI Ratio: **0.50**
- Avg. Credit Score (Defaulters): **559.29**

#### Key Visuals:
- **Loan Defaults by Year, Employment Type, and Purpose**
- Credit Score vs. Default Frequency
- Default Rates across **Income Brackets**, **Age Groups**, and **Loan Purposes**

---

### 🔵 3. Business Performance Analysis
- Total Loan Amount: **₹32.6 Billion**
- Total Interest Income: **₹439.28 Billion**
- Avg. Credit Score (Non-defaulters): **576**
- Avg. Loan Term: **36.03 months**

#### Key Visuals:
- Loan Amount & Interest Income trends (by year)
- Loan Distribution by **Credit Score**, **Employment Type**, and **Income Bracket**

---

## 🛠️ Tools & Technologies Used

| Tool      | Purpose                              |
|-----------|--------------------------------------|
| **Power BI** | Data visualization & dashboard creation |
| **Excel / CSV** | Data transformation, cleaning |
| **DAX** | Calculated columns, measures |
| **Python (optional)** | Preprocessing & data wrangling |

---

## 🚀 Key Insights

- **High-income groups** account for a majority of the loan disbursal and defaults.
- **Unemployed and self-employed individuals** show higher default rates.
- Most defaults come from **medium to high credit score groups**, indicating more than just credit score affects risk.
- **Business and education loans** have higher default risks.
- Interest income peaked in **2015 and 2018**, aligned with peak loan issuance.

---

## 📂 Repository Structure

```
📁 Loan-Portfolio-Dashboard
│
├── 📊 Dashboard Images/
│   ├── Overview_Dashboard.png
│   ├── Risk_Evaluation_Dashboard.png
│   └── Business_Performance_Dashboard.png
│
├── 📄 Dataset (Optional)/
│   └── loan_data.csv
│
├── 📁 PowerBI File/
│   └── Loan_Insights_Dashboard.pbix
│
└── 📄 README.md
```

---

## 💡 Future Improvements

- Add predictive modeling for **default risk classification**.
- Integrate **live data updates** via Power BI Service.
- Expand analysis using **geographical trends** (if location data is available).

---

## 📬 Contact

If you have any questions or suggestions, feel free to reach out:

**Ankit Dutt**  
📧 your-email@example.com  
🔗 [LinkedIn Profile](https://www.linkedin.com/in/yourprofile)  
📍 India  

---

## ⭐️ Give it a Star

If you found this project insightful, please ⭐ the repository to show your support!
