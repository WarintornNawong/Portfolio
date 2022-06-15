# STOCK CLUSTERING FROM TOP 100 THAI STOCKS IN STOCK EXCHANGE OF THAILAND (SET)
## INTRODUCTION
### DATASET 
I used the financial dataset (OHLVC Price and Volume) and thier account information (Balance Sheet, Income Statement and Cashflow Statement) from "YAHOO FINANCE" in yfinance library during 2018 - 2022.
### PART I. Financial Ratio Extraction
In order to cluster the thai stock with similarity-based clustering, I extracted the financial ratios from financial information with the following indicator,
1. **Net Profit Margin (NPM)** : the net income of a company to its net sales to determine operating efficiency.
2. **Gross Profit Margin (GPM)** : compares the gross profit of a company to its net sales to show how much profit a company makes after paying its cost of goods sold.
3. **Return on Equity (ROE)** : measures how efficiently a company is using its equity to generate profit.
4. **Current Ratio (CR)** : to measure a company’s ability to pay off short-term liabilities with current assets.
5. **CXash flow from operating activities-to-Liability Ratio (CFOR)** : measure of the number of times a company can pay off current liabilities with the cash generated in a given period.
6. **Debt-to-Equity Ratio (DE)** : calculates the weight of total debt and financial liabilities against shareholders’ equity.
7. **Interest Coverage Ratio (ICR)** : measure how easily a company can pay its interest expenses.
8. **Payable Turnover Ratio (PTR)** : measures how quickly a business makes payments to creditors and suppliers that extend lines of credit.
9. **Inventory Turnover Ratio (ITR)** : measures how many times a company’s inventory is sold and replaced over a given period.
10. **Receivable Turnover Ratio (RTR)** : measures how many times a company can turn receivables into cash over a given period.
11. **Cash Conversion Cycle (CCC)** : a metric that shows the amount of time it takes a company to convert its investments in inventory to cash.
12. **Compound Annual Growth Rate (CAGR)** : represents one of the most accurate ways to calculate and determine returns for individual assets, investment portfolios.

## PART II. EXPLORATORY DATA ANALYSIS
### Net Profit Margin vs Debt-to-Equity Ratio
![image](https://user-images.githubusercontent.com/104628789/173777268-1a8b7a9b-d84e-454c-8181-4558794ac62c.png)
- Intuch is the one of outstanding stock with high NPM and low DE.
- The most of Thai Stock are scatted between NPM 0 - 0.5 with DE 0 - 2.

### CAGR VS Cash Conversion Cycle
![image](https://user-images.githubusercontent.com/104628789/173777320-38f4fa51-71c8-4b0e-b111-6f337fb60748.png)
- PSG is the one of stock with low Cash Conversion Cycle with high CAGR during 4 years.
- The most of Thai Stock are scatter between 0-0.25 CAGR and 0-200 days cash conversion cycle.

### Inventory TurnoverRatio vs Interest Coverage Ratio
![image](https://user-images.githubusercontent.com/104628789/173777369-3648496b-227b-4618-b525-c7cf449f93dc.png)
- SVH is the lowest ICR compared to the rest of stock

### Receivable Turnover Ratio vs Return of Equity
![image](https://user-images.githubusercontent.com/104628789/173777417-8e3adf37-bfc2-4c6e-9c0a-c7368ed4ba4c.png)
- ADVANCE had the highest ROE with low Receivable turnover
- The most of Thai Stock are scatter between 0.05-0.2 ROE and 0-25 days cash conversion cycle.

### Payable Turnover Ratio vs CashFlowfromOperating-to-Liability Ratio
![image](https://user-images.githubusercontent.com/104628789/173777461-15c15130-8084-46e0-9ce5-d19a9e0cc4e0.png)
- PTW is the highest Cash Flow from Operating with high Payable Turnover Ratio


### Gross Profit Margin vs Current Ratio
![image](https://user-images.githubusercontent.com/104628789/173777496-0f6cc649-1ce1-47d1-a0e0-2eb2e9dddedc.png)
-  BYD is the highest Current Ratio with high Gross Profit Margin

## PART III. Clustering Model Construction
The clustering model I selected to apply for these dataset is specified below,
- KMeans
- Birch
- SpectralClustering
- AgglomerativeClustering
- MiniBatchKMeans
- GaussianMixture

### Optinum Number of Cluster Selection
![image](https://user-images.githubusercontent.com/104628789/173777712-b86b6bdf-3297-41ed-a9cf-af645211d321.png)
I selected is "Elbow Method and Silhoutte Score" to find the optimal number of cluster based on its similarity within cluster and dissimilarity between external stock. The results showed that 6 is the most optimal number between elbow approach and peak silhoutte score so i decided to apply 6 cluster with all model.

## Relative Importance Heat Map
To find the best algorithm for stock clustering, I applied the heat map for calculating the relative importance for individual algorithm to show how they similarize the information.

### I.KMeans
![image](https://user-images.githubusercontent.com/104628789/173777965-e34185f9-9956-45df-b273-f274ac37ab40.png)

### II.Birch
![image](https://user-images.githubusercontent.com/104628789/173778444-9ea1e11b-7d9b-4aae-826d-1aa629509436.png)

### III.Spectral Clustering
![image](https://user-images.githubusercontent.com/104628789/173778590-780aec8e-e7f7-4677-bce5-f79c863ca88b.png)

### IV.AgglomerativeClustering
![image](https://user-images.githubusercontent.com/104628789/173778721-c383eef2-7a82-4761-836a-aaa15fb17e5f.png)

### V.MiniBatch KMeans
![image](https://user-images.githubusercontent.com/104628789/173778967-61a0dfdb-9f8f-4a34-aa0f-9514668923f9.png)

### VI.GaussianMixture
![image](https://user-images.githubusercontent.com/104628789/173779067-4839683e-9f94-4c1a-bfb5-c4083a792b39.png)

## Conclustion
these can be clustered into 6 cluster with the following characteristics and key information,

I. "High Interest Coverage Ratio" : the group of stock 


