# M-pesa-Statement-Analysis- Excel
### User Story
---
 'I gave someone close to me my m-pesa PIN on 5th April 2024 while I was going to a one-month conference in Mumbai city. When I came back on 5th May 2024, I discovered there was a lot of money spent. Kindly let me know how my money was spent, total income and withdrawal, and cashflow based on the running totals. I will appreciate any other information beyond that'. 

### Project Overview
---
 This project is meant to analyze the m-pesa statement as requested by the user in the user story section above. It will analyze how the money was spent from 5th April 2024 to 5th May 2024 (one month). This will be based on the total earnings and withdrawals, cashflow- which is based on the running totals, and any other analysis that will be relevant.
 
### Data Sources
---
**Safaricom**- The m-pesa statement obtained from Safaricom was provided as requested by the client. A data protection sheet was signed to ensure no personal information was leaked to the third party (posting this project here was permitted by the client under some restrictions/guidelines).
The statement had date, code, details, transaction status, paid in, withdrawal and running total columns.

### Tools Used
---
- Adobe Acrobat DC (offline)- PDF conversion
- Excel- Data cleaning, Data preparation, visualization and dashboard

### Data Cleaning and Preparation
---
1. **Adobe Acrobat DC** 
- Converting Data from PDF to Excel Workbook.

2. **Excel**

![blurred](https://github.com/Clifford254KE/M-pesa-Statement-Analysis/assets/140185917/25eebfd3-8b3e-4460-b742-3374a3231818)

*Image of data before transformation (it is blurred to hide some personal information)*

- Replaced missing values with 'zeros' (There were no duplicate values).
- Transformed the 'date' column to contain only day, month, and year.
- Transformed the 'details column' by shortening the long texts through delimiter ( Data > text to column > Delimited).
- Changed withdrawal column from negative values to positive values (using a new column, use function MAX(Cell containing number, -(negative) cell containing number)).
- Another column was created to categorize transactions under the 'detail' column to form different categories of expenses and incomes: shopping, general expenses, black tax, withdrawal -charges, transfer charges, airtime expense, general income, and m-shwari withdrawal (Ctrl H).

![image](https://github.com/Clifford254KE/M-pesa-Statement-Analysis/assets/140185917/c1f919ff-84b0-4c64-9b56-5061ff7a5b06)


*This is the image of cleaned and transformed data ready for analysis*

### Exploratory Data Analysis
---

- What is the total income/withdrawal reported from 4th April 2024 to 5th May 2024?
- What are the expense categories based on how much was spent on each from 4th April 2024 to 5th May 2024?
- What was the cashflow based on the running totals from 4th April 2024 to 5th May 2024?
- What was the trend of withdrawal/income from 4th April 2024 to 5th May 2024?

### Data Analysis
---
Apart from using Excel for data cleaning and preparation, it was also used for data analysis and visualization.
Using a pivot table, questions under exploratory data analysis (EDA) were analyzed and visualized as follows:
- **Question 1**: What is the total income/withdrawal reported from 4th April 2024 to 5th May 2024?

  The analysis below shows that income was higher than withdrawal. This is because it includes even the amount carried forward from the previous month.

![q11](https://github.com/Clifford254KE/M-pesa-Statement-Analysis/assets/140185917/6084735d-ec45-4440-b1b1-6efa716c15ff)
![q12](https://github.com/Clifford254KE/M-pesa-Statement-Analysis/assets/140185917/b8919238-b32f-4bbd-a7bb-9e91df246a6b)

- **Question 2**: What are the expense categories based on how much was spent on each from 4th April 2024 to 5th May 2024?

![q31](https://github.com/Clifford254KE/M-pesa-Statement-Analysis/assets/140185917/a093aafc-25dd-4dbd-8d55-1615b4ead046)
![q32](https://github.com/Clifford254KE/M-pesa-Statement-Analysis/assets/140185917/472b558f-f279-4d7d-934e-d9cc8f8e4f37)

- **Question 3**: What was the cashflow based on the running totals from 4th April 2024 to 5th May 2024?

![q41](https://github.com/Clifford254KE/M-pesa-Statement-Analysis/assets/140185917/98a1ac6f-0adf-4ae0-beaf-d6d673f8f9b3)
![q42](https://github.com/Clifford254KE/M-pesa-Statement-Analysis/assets/140185917/5922ada0-aef8-464c-b8e3-b587e6e83185)

- **Question 4**: What was the trend of withdrawal/income from 4th April 2024 to 5th May 2024?

![q21](https://github.com/Clifford254KE/M-pesa-Statement-Analysis/assets/140185917/399d9f7a-e754-4ea8-8f4c-a8c0c36e9716)
![q22](https://github.com/Clifford254KE/M-pesa-Statement-Analysis/assets/140185917/cb99fa75-c4b9-4091-ac45-b24e680ab6c2)

  **Dashboard**

![Dashboard](https://github.com/Clifford254KE/M-pesa-Statement-Analysis/assets/140185917/5680d3e0-26a9-4a86-bbcd-c06ff36dbd88)

### Results/ Findings
---
1. Total income/withdrawal reported from 4th April 2024 to 5th May 2024: There was a total of ksh. 68,162 and an income of ksh. 69,157. The income amount is higher than the amount spent/withdrawn during the stated period. A total of ksh. 1213 was c/f. Therefore, a total of ksh. 995 available in the account at the end of the month but there was 218 more withdrawn as compared to the income for the month. 
2. Expense categories based on how much was spent on each from 4th April 2024 to 5th May 2024: There were different categories of expenses and amount spent. This has been shown below in a table:

![image](https://github.com/Clifford254KE/M-pesa-Statement-Analysis/assets/140185917/f7aa64aa-26d3-422e-bff6-64632da7cd27)

- **Black tax**: This is the amount of money sent to relatives
- **Airtime expense**: This is the amount of money spent on airtime
- **Withdrawal expense**: Amount withdrawn from m-pesa
- **General expense**: Amount of money spent on maintenance of owners' assets, paying bills (water, electricity, wages, among others), paying for debt or loan.
- **Shopping**: Amount spent on planned shopping (basically buying food)
- **Impulse shopping**: Amount spent on unplanned shopping. NB. It appears as shopping in the dashboard, as required by the client. 
- **Transfer Charges**: Amount deducted when sending money via m-pesa
- **M-shwari**: Amount deposited in M-shwari account. This is savings but the client wanted it to appear as part of the expenses for reasons known to her.

3. Cashflow based on the running totals from 4th April 2024 to 5th May 2024: There is a downward trend as shown by the trendline. This means that there is more money being withdrawn as compared to the amount earned. {NB. The amount earned was more than the amount spent as shown above (check objective 1) because there was some amount of money that was carried forward from the previous month (Question 1).
4. The trend of withdrawal/income from 4th April 2024 to 5th May 2024: Based on the dashboard shown above, the line graph for withdrawals and income are running interchangeably. Sometimes withdrawal is higher than income and vice versa.

### Limitations
---
- M-pesa statement is highly sensitive because it contains personal information and also password protected
- The project was limited to the requirements of the user.
- Some transactions were ambiguous. They were analyzed based on the user's explanation upon inquiry.
### Recommendations
---
- Avoid impulse buying and embrace savings.
- Embrace bulk shopping, it will reduce the amount spent per day for shopping.

**Note**. The project only displays images as shown above. Uploading datasets or Excel worksheets is restricted due to sensitive data in those files.

