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
Apart from using excel for data cleaning and preparation, it was also used for data analysis and visualization.
Using pivot table, questions under exploratory data analysis (EDA) analyzed and visualized as follows:
Question 1: What is the total income/withdrawal reported from 4th April 2024 to 5th May 2024?.

![q11](https://github.com/Clifford254KE/M-pesa-Statement-Analysis/assets/140185917/6084735d-ec45-4440-b1b1-6efa716c15ff)
![q12](https://github.com/Clifford254KE/M-pesa-Statement-Analysis/assets/140185917/b8919238-b32f-4bbd-a7bb-9e91df246a6b)

Question 2: What are the expense categories based on how much was spent on each from 4th April 2024 to 5th May 2024?.

![q31](https://github.com/Clifford254KE/M-pesa-Statement-Analysis/assets/140185917/a093aafc-25dd-4dbd-8d55-1615b4ead046)
![q32](https://github.com/Clifford254KE/M-pesa-Statement-Analysis/assets/140185917/472b558f-f279-4d7d-934e-d9cc8f8e4f37)

Question 3: What was the cashflow based on the running totals from 4th April 2024 to 5th May 2024?.

![q41](https://github.com/Clifford254KE/M-pesa-Statement-Analysis/assets/140185917/98a1ac6f-0adf-4ae0-beaf-d6d673f8f9b3)
![q42](https://github.com/Clifford254KE/M-pesa-Statement-Analysis/assets/140185917/5922ada0-aef8-464c-b8e3-b587e6e83185)

Question 4: What was the trend of withdrawal/income from 4th April 2024 to 5th May 2024?.

![q21](https://github.com/Clifford254KE/M-pesa-Statement-Analysis/assets/140185917/399d9f7a-e754-4ea8-8f4c-a8c0c36e9716)
![q22](https://github.com/Clifford254KE/M-pesa-Statement-Analysis/assets/140185917/cb99fa75-c4b9-4091-ac45-b24e680ab6c2)

Dashboard

![Dashboard](https://github.com/Clifford254KE/M-pesa-Statement-Analysis/assets/140185917/5680d3e0-26a9-4a86-bbcd-c06ff36dbd88)



