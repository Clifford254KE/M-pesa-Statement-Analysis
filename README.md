# M-pesa-Statement-Analysis
### User Story
---
 'I gave someone close to me my m-pesa PIN on 5th April 2024 while I was going to a one-month conference in Mumbai city. When I came back on 5th May 2024, I discovered there was a lot of money spent. Kindly let me know how my money was spent, total income and withdrawal, and cashflow based on the running totals. I will appreciate any other information beyond that'. 

### Project Overview

 This project is meant to analyze the m-pesa statement as requested by the user in the user story section above. It will analyze how the money was spent from 5th April 2024 to 5th May 2024 (one month). This will be based on the total earnings and withdrawals, cashflow which is based on the running totals, and any other analysis that will be relevant.

### Data Sources
Safaricom- The m-pesa statement obtained from Safaricom was provided as requested by the client. A data protection sheet was signed to ensure no personal information was leaked to the third party (posting this project here was permitted by the client under some restrictions/guidelines)

### Tools Used
Adobe Acrobat DC (offline)- PDF conversion
Excel- Data cleaning, Data preparation, visualization and dashboard

### Data Cleaning and Preparation
Adobe Acrobat DC 
Converting Data from PDF to Excel Workbook.

Excel

![blurred](https://github.com/Clifford254KE/M-pesa-Statement-Analysis/assets/140185917/25eebfd3-8b3e-4460-b742-3374a3231818)

Image of data before transformation (it is blurred to hide some personal information)

Removed duplicates and replaced missing values with 'zeros'.
Transformed the 'date' column to contain only day, month, and year.
Transformed the 'details column' by shortening the long texts through delimiter ( Data > text to column > Delimited).
Changed withdrawal column from negative values to positive values (using a new column, use function MAX(Cell containing number, -(negative) cell containing number)).
Another column was created to categories transactions under the 'detail' column to form different kinds of expenses and incomes: shopping, general expenses, black tax, withdrawal charges, transfer charges, airtime expense, general income, m-shwari withdrawal (Ctrl H).

![image](https://github.com/Clifford254KE/M-pesa-Statement-Analysis/assets/140185917/c1f919ff-84b0-4c64-9b56-5061ff7a5b06)


This is the image of cleaned and transformed data ready for analysis

### Exploratory Data Analysis

What is the total income/withdrawal reported from 4th April 2024 to 5th May 2024?.
What are the expense categories based on how much was spent on each from 4th April 2024 to 5th May 2024?.
What was the cashflow based on the running totals from 4th April 2024 to 5th May 2024?.
What was the trend of withdrawal/income from 4th April 2024 to 5th May 2024?.

### Data Analysis


