# COMPANY BANKRUPTCY PREDICTION
### INTRODUCTION

Bankruptcy prediction is a technique for predicting bankruptcy and various financial conditions of state-owned, public firm or any company through the financial ratio from balance sheet, income and cashflow statement of company. The financial ratios could represent the company status, risk and health. The different of private and public firm is the different accounting regulation and comformation which lead to the different in availability of data. However, the approach to predict to measure financial distress is identical.

This technique could enable lenders and investors to evaluate the likelihood of a company going bankrupt, to provide a wise investment decision in a survivable company with past or current company financial status and signal government to subsidize or bail out in advance to reduce the impact of financial crisis.


### DATASET
The data I utilized to train model were derived from Kaggle Dataset in [Company Bankruptcy Prediction](https://www.kaggle.com/datasets/fedesoriano/company-bankruptcy-prediction). The data were collected from the Taiwan Economic Journal for the years 1999 to 2009. Company bankruptcy was defined based on the business regulations of the Taiwan Stock Exchange with Source from Deron Liang and Chih-Fong Tsai, National Central University, Taiwan. The data have 96 attribute including the bankruptcy label. The example of attribute is specified in following bullet,

**Attribute Information**

- Y - Bankrupt?: Class label
- X1 - ROA(C) before interest and depreciation before interest: Return On Total Assets(C)
- X2 - ROA(A) before interest and % after tax: Return On Total Assets(A)
- X3 - ROA(B) before interest and depreciation after tax: Return On Total Assets(B)
- X4 - Operating Gross Margin: Gross Profit/Net Sales

you can find all full detail of attribute [here](https://www.kaggle.com/datasets/fedesoriano/company-bankruptcy-prediction).


## PART III Model Development
i select the class
1. Random Forest
2. Gradient Boosting
3. AdaBoost
