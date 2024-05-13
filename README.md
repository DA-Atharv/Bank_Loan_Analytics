# Bank_Loan_Analytics
# Project Overview:
The Bank Loan Portfolio Analysis project aims to leverage SQL queries and Power BI visualization tools to provide comprehensive insights into the bank's loan portfolio. By analyzing various loan metrics, the project seeks to enhance decision-making processes, mitigate risks, and optimize loan management strategies.

# Significance:
Understanding the bank's loan portfolio is crucial for effective decision-making in banking institutions. Analyzing loan data helps in assessing the distribution of loans across different categories, evaluating loan performance metrics, identifying trends, and optimizing lending practices. This project enables stakeholders to make informed decisions related to loan management, risk mitigation, and portfolio optimization, ultimately contributing to the bank's overall financial health and performance.

# Project Contents:
| Files | Description |
|-------| ------------|
| [Data](https://github.com/DA-Atharv/Bank_Loan_Analytics/tree/main/DATA) | This folder houses a comprehensive collection of Bank Loan Details data . |
| [Power BI File](https://github.com/DA-Atharv/Bank_Loan_Analytics/blob/main/Power%20Bi%20Dashboard%20File.pbix) | This folder houses a comprehensive collection of Power BI Analysis & Dashboard for Bank Loan Analytics. |
| [Dashboard Images](https://github.com/DA-Atharv/Bank_Loan_Analytics/tree/main/Dashboard_Images ) | This folder houses Images of Bank Analytics Dashboard. |
| [SQL_Queries.md](https://github.com/DA-Atharv/Bank_Loan_Analytics/blob/main/SQL_Queries.md) | Contains SQl Queries perform to analyse Bank Loan Analytics. |
| [README.md](https://github.com/DA-Atharv/Bank_Loan_Analytics/edit/main/README.md) | This is the Readme file of the project. |

# Project Analysis: 1) Power BI Analysis:
In the Power BI analysis for the Bank Loan Portfolio project, data cleaning and transformation were initially conducted using Power Query tools. Following this, DAX measures and KPIs were created to calculate key metrics like interest rates and loan application percentages. Interactive dashboards were then designed with a range of visualizations such as pie charts, bar graphs, line/area chats. Additionally, bookmarks and page navigations were implemented to enhance user experience, allowing for seamless navigation between different sections of the dashboard. Conditional formatting was also applied to highlight important insights, ensuring stakeholders could easily interpret loan portfolio data for informed decision-making and risk assessment.
### Dashboard 1: Summary
+ Provides key loan-related metrics and KPIs for monitoring lending activities.
+ Distinguishes between good and bad loans for risk assessment.
+ Offers insights into loan performance and borrower behavior.
+ Tracks total loan applications, funded amount, and amount received.
+ Calculates average interest rate and debt-to-income ratio (DTI).
+ Analyzes good loan application percentage and bad loan application percentage.
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/6e83040b-0929-449a-a9fc-837853783447)

### Dashboard 2: Overview
+ Presents loan-related information and trends through various visualizations.
+ Includes charts on monthly trends, regional analysis, loan terms, employee length, loan purposes, and home ownership.
+ Aids in comprehensive analysis and strategic decision-making.
+ Visualizes changes in loan applications, funded amount, and amount received over time.
+ Identifies regional variations in loan activity.
+ Illustrates loan distribution based on term lengths, employment length, loan purposes, and home ownership.
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/dccfd1bb-5cc5-4b3d-9fa0-94b735530b58)

### Dashboard 3: Details
+ Offers a comprehensive view of loan portfolio details and borrower profiles.
+ Includes metrics on loan performance, borrower characteristics, and loan status.
+ Facilitates informed decision-making and risk assessment.
+ Summarizes total loan applications, funded amount, and amount received.
+ Presents demographic information and borrower characteristics.
+ Tracks loan profitability, borrower financial health, and repayment behavior.
+ Provides a detailed report categorizing loans by status for easy tracking and analysis.
![image](https://github.com/DA-Atharv/Bank_Loan_Analytics/assets/159448408/529a2927-7cba-41d5-a309-86d1a2d6ff4b)

# Project Analysis: 2) SQL Analysis: 
In executing the Bank Loan Portfolio Analysis project, various SQL techniques were utilized. Aggregation functions computed key indicators, joins combined data, and CASE WHEN statements facilitated categorization. The GROUP BY clause aggregated data, the WHERE clause filtered it, and the DATEFORMAT function aided in trend analysis. These SQL techniques enabled the extraction of valuable insights, guiding decision-making within the banking institution. Enhanced risk management and portfolio optimization strategies were achieved, driven by data-driven insights derived from comprehensive loan data analysis.

### Loan Applications: 
+ Total loan applications | Monthly loan applications | Previous month's monthly loan applications.

### Funding Analysis:
+ Total funded amount | Monthly total funded amount | Previous month's total funded amount.

### Repayment Analysis:
+ Total amount received | Monthly total amount received | Previous month's total amount received.

### Interest Rate Analysis:
+ Average interest rate | Monthly average interest rate | Previous month's average interest rate.

### Debt-to-Income Ratio (DTI) Analysis:
+ Average DTI | Monthly average DTI | Previous month's average DTI.

### Loan Quality Analysis:
+ Good loan percentage | Bad loan percentage.

### Loan Status Overview:
+ Loan status summary | Monthly loan status summary.

### Monthly Trends Analysis:
+ Monthly trend by issue date.

### Regional Analysis:
+ Regional analysis by state.

### Loan Characteristics Analysis:
+ Loan term analysis | Employee length analysis | Loan purpose analysis | Homeownership analysis.

### Monthly Performance Comparison:
+ Month over month total funded amount | Month over month average interest rate.
