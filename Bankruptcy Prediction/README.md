# COMPANY BANKRUPTCY PREDICTION
### INTRODUCTION

Bankruptcy prediction is a technique for predicting bankruptcy and various financial conditions of state-owned, public firm or any company through the financial ratio from balance sheet, income and cashflow statement of company. The financial ratios could represent the company status, risk and health. The different of private and public firm is the different accounting regulation and comformation which lead to the different in availability of data. However, the approach to predict to measure financial distress is identical.

This technique could enable lenders and investors to evaluate the likelihood of a company going bankrupt, to provide a wise investment decision in a survivable company with past or current company financial status and signal government to subsidize or bail out in advance to reduce the impact of financial crisis.


### DATASET
The data I utilized to train model were derived from Kaggle Dataset in [Company Bankruptcy Prediction](https://www.kaggle.com/datasets/fedesoriano/company-bankruptcy-prediction). The data were collected from the Taiwan Economic Journal for the years 1999 to 2009. Company bankruptcy was defined based on the business regulations of the Taiwan Stock Exchange with Source from Deron Liang and Chih-Fong Tsai, National Central University, Taiwan. The data have 96 attribute including the bankruptcy label. The example of attribute is specified in following bullet,

## POST-FEATURE SELECTION
the financial ration of the company will have more than 90 parameter which might cause inconveniet to construct high efficiency model so I decided to apply the feature engineering - Correlation-based and Modelbased feature selection. With the model based feature selection, I apply the random forest classifier alongside with Recursive Feature Elimination (RFE) to find the most optimal accuracy with appropriate number of features. 

![image](https://user-images.githubusercontent.com/104628789/170246962-9d94e1b6-1b6e-4e34-aaa8-6f86c6a11ff9.png)

The figure indicated that the most optimal number of parameter is 30 feature to contribute the highest accuracy among those number.

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

### Observation 
These parameter showed obviously the different between bankrupt firm and non-bankrupt firm for example the company that went bankrupt would have high debt, liability  and low cash or liquidity which might lead to low income. However, some key employee-related indicator such as revenue per person or operating profit per person could not differentiate or signify the probility of bankruptcy in any firm.

## Model Construction
I have selected the classification model from sklearn library to construct the model and measure performance the model in metrics - "Accuracy, Precision, Recall, F1 and ROC-AUC SCore". Due to high imbalance data, I decided to generate the data based on "Oversampling Apprach - SMOTE" to equalize the number of normal and bankrupted firm, Moreover, we have tuned the model hyperparameter of each model.

1. Random Forest Classifier
2. Gradient Boosting Classifier
3. AdaBoost Classifier

![image](https://user-images.githubusercontent.com/104628789/170244902-90f6a544-476e-4940-b542-1b10c7e1219f.png)

