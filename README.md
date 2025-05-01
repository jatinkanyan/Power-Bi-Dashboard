# 📊 Power BI Dashboard: Unlocking Financial Insights in Banking Data

## 🧾 Project Overview

This Power BI project explores banking transaction and account datasets to uncover patterns, evaluate customer behavior, and support data-driven financial decision-making. It integrates two datasets—transactions and account details—and visualizes key KPIs and trends using interactive visuals and advanced DAX calculations.

The goal is to provide a 360-degree view of customer activity, risk exposure, and branch performance while demonstrating best practices in data modeling, transformation, and dashboard design.

---

## 📁 Datasets Used

### 1. `BankingDataset 1.xlsx` – **Transactions Data**
| Column             | Description                                 |
|--------------------|---------------------------------------------|
| TransactionID      | Unique transaction identifier               |
| AccountNumber      | Customer account number                     |
| TransactionType    | Deposit, Withdrawal, Transfer, etc.         |
| Amount             | Transaction amount                          |
| TransactionDate    | Date of transaction                         |
| BranchCode         | Originating branch                          |
| Currency           | Currency used                               |
| TransactionTime    | Hour of transaction (0–23)                  |

### 2. `BankingDataset 2.xlsx` – **Account Data**
| Column               | Description                                      |
|----------------------|--------------------------------------------------|
| AccountNumber        | Unique customer account number                   |
| AccountHolder        | Name of the account holder                       |
| AccountType          | Credit, Loan, Checking, Savings                  |
| Balance              | Current account balance                          |
| InterestRate         | Account-specific interest rate                   |
| CreditScore          | Customer credit score                            |
| OpeningDate          | Date account was opened                          |
| LoanAmount           | Loan issued to the customer                      |
| AccountHolderDetails | Sector, residence duration, and city (parsed)    |

---

## 📊 Dashboard Highlights

The dashboard is designed using Power BI and includes:

### 📌 KPIs
- 🔢 Total Transactions: **918**
- 💳 Average Credit Score: **575.3**
- 💰 Total Transaction Value: **₹46.4M+**
- 🧾 Average Account Balance: **₹23.9K**

### 📊 Visual Insights
- Transaction breakdown: Incoming, Outgoing, Cash Out
- Balances by account type
- High-Value vs Normal transaction flagging
- Customer risk segmentation: Low, Medium, High
- Time-of-day patterns in transaction activity
- Quarterly transaction trend analysis
- Interest rate vs balance correlation
- Credit score vs loan amount relationship

### 🏦 Branch Performance
- Branch **479** leads in transaction volume and performance score (**1.00**)
- Branch analysis includes transaction count and total loan volume

### 📅 Time Intelligence
- Transaction volume by **quarter**
- Account age and loyalty indicators
- Year-wise loan disbursement (2023–2025)

---

## ✅ Analytical Questions Answered

> The following analyses were conducted and visualized in the dashboard:

1. **Data Importing & Cleaning**: Null values in TransactionType, Currency, and Balance columns were handled. Missing AccountHolder values flagged.  
2. **Merging Datasets**: Linked using `AccountNumber`.  
3. **Handling Missing & Irrelevant Data**: Cleaned, duplicates removed, and non-informative fields excluded.  
4. **Data Type Conversion**: Dates, currency, and categorical fields normalized.  
5. **Categorizing Transaction Types**: Grouped into categories like Incoming, Outgoing, Payment, Transfer, Other.  
6. **Avg Account Balance**: *Savings accounts* have the highest average balances.  
7. **Currency Normalization**: Converted using fixed rates to INR for comparison.  
8. **Branch Activity**: Branch 479 leads in transaction count.  
9. **Interest vs Balance Correlation**: Extremely low correlation (**0.01**).  
10. **Loan Amount vs Credit Score**: No meaningful correlation (**0.01**).  
11. **Transaction Trends**: Highest activity in Q2, with visible seasonal variation.  
12. **Customer Loyalty**: Several accounts aged 10+ years; total account-years = 3864.  
13. **High-Value Transactions**: 8.06% of all transactions, based on statistical outlier thresholds.  
14. **Time-of-Day Analysis**: Mornings and afternoons most active.  
15. **Credit Score Distribution**: Mostly Fair to Good; few Excellent or Poor.  
16. **Account Age vs Balance Correlation**: Negligible (**0.005**).  
17. **Branch Ratings**: Based on transaction volume and loan disbursement.  
18. **Info Extraction**: Parsed `AccountHolderDetails` into Sector, Years at Residence, City.  


---


🛠️ Tools Used
Power BI Desktop

DAX (for measures and custom columns)

Power Query Editor (for transformation and cleaning)

Excel (.xlsx source files)

🚀 How to Use
Download BankingDashboard.pbix and both .xlsx datasets from this repository.

Open in Power BI Desktop.

Use slicers to filter by Account Type, BranchCode, Currency, and Date.

Interact with visuals to explore branch performance, customer trends, and risk profiles.

✍️ Author
Jatin Kanyan
📧 yourJatinkanyan11@gmail.com
🔗 GitHub: 


