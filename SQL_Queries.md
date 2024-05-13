## 1) Total Loan Applications:
```sql
select count(id) as total_loan_application from bank_loan
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/990935c7-a885-45a0-999b-fe9c4d16bb5b)

## 2) MTD Loan Applications:
```sql
select count(id) as MTD_Total_Loan_Application from bank_loan
where month(issue_date) = 12 and year(issue_date) = 2021
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/aafc9a90-6ce4-405c-80c4-b339d31e4552)

### 3) PMTD Loan Applications:
```sql
select sum(loan_amount) as MTD_Total_Funded_Amount from bank_loan
where month(issue_date) = 12 and year(issue_date) = 2021
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/7cc298b0-af1e-4f22-af61-74a4b4bee9e2)

# 4) Total Funded Amount:
```sql
select sum(loan_amount) as Total_Funded_Amount from bank_loan
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/bc2565a7-8eda-40cf-a2bf-612aad8f5670)

# 5) MTD Total Funded Amount:
```sql
select sum(loan_amount) as MTD_Total_Funded_Amount from bank_loan
where month(issue_date) = 12 and year(issue_date) = 2021
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/74c01f31-0755-4bcb-9571-14e980cdae5f)

# 6) PMTD Total Funded Amount:
```sql
select sum(loan_amount) as PMTD_Total_Funded_Amount from bank_loan
where month(issue_date) = 11 and year(issue_date) = 2021
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/00219217-385a-46cd-84ed-6496bf138df5)

# 7) Total Amount Received:
```sql
select sum(total_payment) as Total_Amount_Receieved from bank_loan
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/836bcbec-0355-40b9-8bfa-c6302924f52c)

# 8) MTD Total Amount Received:
```sql
select sum(total_payment) as MTD_Total_Amount_Receieved from bank_loan
where month(issue_date) = 12 and year(issue_date) = 2021
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/afe22ed4-e3a5-4385-84a9-711972dfcbf8)

# 9) PMTD Total Amount Received:
```sql
select sum(total_payment) as PMTD_Total_Amount_Receieved from bank_loan
where month(issue_date) = 11 and year(issue_date) = 2021
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/6bf649f3-5e94-45a9-ba7c-fd2b521ca87c)

# 10) Average Interest Rate:
```sql
select round(avg(int_rate) * 100, 2) as Average_Interest_Rate from bank_loan
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/bd7bac7c-296b-4b3e-b73e-89466f3e09a0)

# 11) MTD Average Interest:
```sql
select round(avg(int_rate) * 100, 2) as MTD_Average_Interest_Rate from bank_loan
where month(issue_date) = 12 and year(issue_date) = 2021
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/4f93d172-f793-477f-bfca-e0af20b701df)

# 12) PMTD Average Interest:
```sql
select round(avg(int_rate) * 100, 2) as PMTD_Average_Interest_Rate from bank_loan
where month(issue_date) = 11 and year(issue_date) = 2021
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/bf532ce0-adf3-4f34-a791-6041f3539737)

# 13) Average DTI:
```sql
select round(avg(dti) * 100, 2) as Average_DTI from bank_loan
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/2189ea28-6239-4c1c-8b26-ca77f8ae4628)

# 14) MTD Average DTI:
```sql
select round(avg(dti) * 100, 2) as MTD_Average_DTI from bank_loan
where month(issue_date) = 12 and year(issue_date) = 2021
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/d547c9da-61c1-4eb5-8c1c-b60b0fa9b70c)

# 15) PMTD Average DTI:
```sql
select round(avg(dti) * 100, 2) as PMTD_Average_DTI from bank_loan
where month(issue_date) = 11 and year(issue_date) = 2021
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/fd19ca88-05b7-447b-a295-102bc1c00180)

# 16) Good Loan Percentage:
```sql
select(count(case when loan_status = 'Fully Paid' or loan_status = 'Current' then id end) * 100.0)/count(id)
as Good_Loan_percentage
from bank_loan
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/cc6afe50-6cd6-48d5-9cbb-946a373a0f46)

# 17) Good Loan Applications:
```sql
select count(id) as Good_Loan_Applications from bank_loan
where loan_status = 'Fully Paid' or loan_status = 'Current'
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/497e7fd7-0672-42c1-8819-316c4541868e)

# 18) Good Loan Funded Amount:
```sql
select sum(loan_amount) as Good_Loan_Funded_Amount from bank_loan
where loan_status = 'Fully Paid' or loan_status = 'Current'
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/63802d3a-1495-4264-9ac0-2faec2d1ef7a)

# 19) Good Loan Amount Received:
```sql
select sum(total_payment) as Good_Loan_Funded_Amount from bank_loan
where loan_status = 'Fully Paid' or loan_status = 'Current'
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/b4da0934-d15b-4b76-adf6-6a66ef166e92)

# 20) Bad Loan Percentage:
```sql
select(count(case when loan_status = 'Charged Off' or loan_status = 'Current' then id end) * 100.0)/count(id)
as Bad_Loan_percentage
from bank_loan
```
# 21) Bad Loan Applications:
```sql
select count(id) as Bood_Loan_Applications from bank_loan
where loan_status = 'Charged Off' 
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/358c32e7-9c4e-4548-ae4b-781cfdf5eb98)

# 22) Bad Loan Funded Amount:
```sql
select sum(loan_amount) as Bood_Loan_Funded_Amount from bank_loan
where loan_status = 'Charged Off' 
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/3dd094ff-e988-4fdd-8515-0be394f27685)

# 23) Bad Loan Amount Received:
```sql
select sum(total_payment) as Bad_Loan_Received_Amount from bank_loan
where loan_status = 'Charged Off' 
```

# 24) LOAN STATUS:
```sql
select loan_status as Loan_Status, count(id) as Total_Applications, sum(total_payment) as Total_Amount_Recieved,
sum(loan_amount) as Total_Funded_Amount, avg(int_rate * 100) as Interest_Rate, avg(dti * 100) as DTI
from bank_loan group by loan_status
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/cc654921-f3e4-4fe6-9b23-afa66e5a5826)

# 25) 
```sql
select loan_status as Loan_Status, sum(total_payment) as MTD_Total_Amount_Recieved,
sum(loan_amount) as MTD_Total_Funded_Amount,
from bank_loan where month(issue_date) = 12
group by loan_status
```
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/8b1e9a95-a4ff-4df7-a4a7-bea48b7e1c3a)















