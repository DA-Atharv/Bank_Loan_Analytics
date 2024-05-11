# 1) Total Loan Applications:
```sql
select count(id) as total_loan_application from bank_loan
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/990935c7-a885-45a0-999b-fe9c4d16bb5b)

# 2) MTD Loan Applications:
```sql
select count(id) as MTD_Total_Loan_Application from bank_loan
where month(issue_date) = 12 and year(issue_date) = 2021
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/aafc9a90-6ce4-405c-80c4-b339d31e4552)
