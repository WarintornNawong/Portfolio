# COMPANY BANKRUPTCY PREDICTION
### INTRODUCTION

Bankruptcy prediction is a technique for predicting bankruptcy and various financial conditions of state-owned, public firm or any company through the financial ratio from balance sheet, income and cashflow statement of company. The financial ratios could represent the company status, risk and health. The different of private and public firm is the different accounting regulation and comformation which lead to the different in availability of data. However, the approach to predict to measure financial distress is identical.

This technique could enable lenders and investors to evaluate the likelihood of a company going bankrupt, to provide a wise investment decision in a survivable company with past or current company financial status and signal government to subsidize or bail out in advance to reduce the impact of financial crisis.


### DATASET
The data I utilized to train model were derived from Kaggle Dataset in [Company Bankruptcy Prediction](https://www.kaggle.com/datasets/fedesoriano/company-bankruptcy-prediction). The data were collected from the Taiwan Economic Journal for the years 1999 to 2009. Company bankruptcy was defined based on the business regulations of the Taiwan Stock Exchange with Source from Deron Liang and Chih-Fong Tsai, National Central University, Taiwan. The data have 96 attribute including the bankruptcy label. The example of attribute is specified in following bullet,

## PART I FEATURE SELECTION

## POST-FEATURE SELECTION
With the results of RFE, They come out 30 key attribute which signify the bankruptcy status is the following detail,
- ROA(C) before interest and depreciation before interest: Return On Total Assets(C)
- Non-industry income and expenditure/revenue: Net Non-operating Income Ratio
- Interest-bearing debt interest rate: Interest-bearing Debt/Equity
- Net Value Per Share (B): Book Value Per Share(B)
- Persistent EPS in the Last Four Seasons: EPS-Net Income
- Net Value Growth Rate: Total Equity Growth
- Total Asset Return Growth Rate Ratio: Return on Total Asset Growth
- Quick Ratio: Acid Test
- Interest Expense Ratio: Interest Expenses/Total Revenue
- Total debt/Total net worth: Total Liability/Equity Ratio
- Debt ratio %: Liability/Total Assets
- Borrowing dependency: Cost of Interest-bearing Debt
- Accounts Receivable Turnover
- Average Collection Days: Days Receivable Outstanding
- Fixed Assets Turnover Frequency
- Revenue per person: Sales Per Employee
- Operating profit per person: Operation Income Per Employee
- Working Capital to Total Assets
- Cash/Total Assets
- Cash/Current Liability
- Inventory/Working Capital
- Working Capital/Equity
- Total income/Total expense
- Total assets to GNP price
- No-credit Interval
- Net Income to Stockholder's Equity
- Degree of Financial Leverage (DFL)
- Interest Coverage Ratio (Interest expense to EBIT)
- Equity to Liability


![image](https://user-images.githubusercontent.com/104628789/170217519-697a1134-913e-4391-b70f-f93828fa3683.png)
![image](https://user-images.githubusercontent.com/104628789/170217771-176eab65-1d24-4ac4-b8f8-cedce72cbea9.png)
![image](https://user-images.githubusercontent.com/104628789/170218027-7ef70163-6ef7-4671-be5e-3fc07cbbf8ec.png)
![image](https://user-images.githubusercontent.com/104628789/170218398-5acb6170-b7a3-4a7d-ab2e-505c4376c9b0.png)
![image](https://user-images.githubusercontent.com/104628789/170218459-0d0ea3f0-19e5-4429-9940-d9a482a23734.png)
![image](https://user-images.githubusercontent.com/104628789/170218513-3fcd4114-b978-4fc7-8ed5-c3571a5abf28.png)
![image](https://user-images.githubusercontent.com/104628789/170218556-07d90a07-0dce-48c3-8d8d-a1da60e01ee0.png)
![image](https://user-images.githubusercontent.com/104628789/170218613-d54f0ff0-4228-42fc-bee8-78517ad7d25c.png)
![image](https://user-images.githubusercontent.com/104628789/170218657-f10c9a9e-6656-49ba-ad59-8d26847aa606.png)
![image](https://user-images.githubusercontent.com/104628789/170218709-1d26771d-bd9b-466a-8d60-d113d22102ba.png)
![image](https://user-images.githubusercontent.com/104628789/170218756-2bc476a6-50be-47a5-b8a4-527d06014d40.png)
![image](https://user-images.githubusercontent.com/104628789/170218793-59fd4d42-6dac-4e01-8c7e-90a65ecdccaf.png)
![image](https://user-images.githubusercontent.com/104628789/170218885-d6c1ba7a-00ab-4b5a-8eb4-a161eeb66ea7.png)
![image](https://user-images.githubusercontent.com/104628789/170218940-a07bebee-8315-419c-8f9e-0776f4513e4d.png)
![image](https://user-images.githubusercontent.com/104628789/170220027-cc7115d4-e9e2-4b0e-9c87-5f066b559639.png)


## PART III Model Development
i select the class
1. Random Forest
2. Gradient Boosting
3. AdaBoost
