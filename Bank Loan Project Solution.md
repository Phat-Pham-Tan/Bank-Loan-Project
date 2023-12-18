# Solution

<p align="right"> Using Microsoft SQL Server </p>

##   A. BANK LOAN REPORT | SUMMARY

### _*KPI’s*_:

### 1. Total Loan Applications

```sql
SELECT COUNT(id) AS Total_Applications 
FROM financial_loan_data
```
#### Result 
| Total_Applications |
|---------------------|
|        38576        |

### 2. MTD Total Amount Received - MTD is "Month-to-Date"
```sql
SELECT COUNT(id) AS Total_Applications 
FROM financial_loan_data
WHERE MONTH(issue_date) = 12
```
#### Result 
| Total_Applications |
|---------------------|
|        4314        |

### 3. PMTD Loan Applications - PMTD is "Processed Month-to-Date"
```sql
SELECT COUNT(id) AS Total_Applications 
FROM financial_loan_data
WHERE MONTH(issue_date) = 11
```
#### Result 
| Total_Applications |
|---------------------|
|        4035        |

### 4. Total Funded Amount
```sql
SELECT SUM(loan_amount) AS Total_Funded_Amount 
FROM financial_loan_data
```
#### Result 
| Total_Funded_Amount  |
|---------------------|
|        435757075        |



