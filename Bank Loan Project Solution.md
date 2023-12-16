# Bank Loan Project Solution

<p align="right"> Using Microsoft SQL Server </p>

## BANK LOAN REPORT | SUMMARY
## KPI’s:

### What is the total number of loan applications?

```sql
SELECT COUNT(id) AS Total_Applications 
FROM financial_loan_data
```
#### Result 
| Total_Applications |
|---------------------|
|        38576        |
