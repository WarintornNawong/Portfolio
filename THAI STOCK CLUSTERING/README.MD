# STOCK CLUSTERING FROM TOP 100 THAI STOCKS IN STOCK EXCHANGE OF THAILAND (SET)
## INTRODUCTION
### DATASET 
I used the financial dataset (OHLVC Price and Volume) and thier account information (Balance Sheet, Income Statement and Cashflow Statement) from "YAHOO FINANCE" in yfinance library.
### PART I. Financial Ratio Extraction
In order to cluster the thai stock with similarity-based clustering, I extracted the financial ratios from financial information with the following indicator,
1. Net Profit Margin (NPM)
2. Gross Profit Margin (GPM)
3. Return on Equity (ROE)
4. Current Ratio (CR)
5. cash flow from operating activities-to-Liability Ratio (CFOR)
6. Debt-to-Equity Ratio (DE)
7. Interest Coverage Ratio (ICR)
8. Payable Turnover Ratio (PTR)
9. Inventory Turnover Ratio (ITR)
10. Receivable Turnover Ratio (RTR)
11. Cash Conversion Cycle (CCC)
12. Compound Annual Growth Rate (CAGR)

## PART II. EXPLORATORY DATA ANALYSIS
![image](https://user-images.githubusercontent.com/104628789/173777268-1a8b7a9b-d84e-454c-8181-4558794ac62c.png)
![image](https://user-images.githubusercontent.com/104628789/173777320-38f4fa51-71c8-4b0e-b111-6f337fb60748.png)
![image](https://user-images.githubusercontent.com/104628789/173777369-3648496b-227b-4618-b525-c7cf449f93dc.png)
![image](https://user-images.githubusercontent.com/104628789/173777417-8e3adf37-bfc2-4c6e-9c0a-c7368ed4ba4c.png)
![image](https://user-images.githubusercontent.com/104628789/173777461-15c15130-8084-46e0-9ce5-d19a9e0cc4e0.png)
![image](https://user-images.githubusercontent.com/104628789/173777496-0f6cc649-1ce1-47d1-a0e0-2eb2e9dddedc.png)

- Observation

## PART III. Clustering Model Construction
The clustering model I selected to apply for these dataset is
- KMeans
- Birch
- SpectralClustering
- AgglomerativeClustering
- MiniBatchKMeans
- GaussianMixture

![image](https://user-images.githubusercontent.com/104628789/173777712-b86b6bdf-3297-41ed-a9cf-af645211d321.png)

- **I.KMeans**
![image](https://user-images.githubusercontent.com/104628789/173777965-e34185f9-9956-45df-b273-f274ac37ab40.png)

- **II.Birch**
![image](https://user-images.githubusercontent.com/104628789/173778444-9ea1e11b-7d9b-4aae-826d-1aa629509436.png)

- **III.Spectral Clustering**
![image](https://user-images.githubusercontent.com/104628789/173778590-780aec8e-e7f7-4677-bce5-f79c863ca88b.png)

- **IV.AgglomerativeClustering**
![image](https://user-images.githubusercontent.com/104628789/173778721-c383eef2-7a82-4761-836a-aaa15fb17e5f.png)

- **V.MiniBatch KMeans**
![image](https://user-images.githubusercontent.com/104628789/173778967-61a0dfdb-9f8f-4a34-aa0f-9514668923f9.png)

- **VI.GaussianMixture**
![image](https://user-images.githubusercontent.com/104628789/173779067-4839683e-9f94-4c1a-bfb5-c4083a792b39.png)



