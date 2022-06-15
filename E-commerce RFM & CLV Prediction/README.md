# E-commerce Customer Clustering and Customer Lifetime Value Prediction
## Introduction
### DATASET 
- Data Set Information:

a transnational data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail.The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers. 

- Attribute Information:

1. **InvoiceNo**: Invoice number. Nominal, a 6-digit integral number uniquely assigned to each transaction. If this code starts with letter 'c', it indicates a cancellation.
2. **StockCode**: Product (item) code. Nominal, a 5-digit integral number uniquely assigned to each distinct product.
3. **Description**: Product (item) name. Nominal.
4. **Quantity**: The quantities of each product (item) per transaction. Numeric.
5. **InvoiceDate**: Invice Date and time. Numeric, the day and time when each transaction was generated.
6. **UnitPrice**: Unit price. Numeric, Product price per unit in sterling.
7.**CustomerID**: Customer number. Nominal, a 5-digit integral number uniquely assigned to each customer.
8. **Country**: Country name. Nominal, the name of the country where each customer resides.

## PART I. DATASET INFORMATION
![image](https://user-images.githubusercontent.com/104628789/173783431-283a1b05-7c20-4868-9383-4e2ee779b6f5.png)
![image](https://user-images.githubusercontent.com/104628789/173783513-a65e696b-f90d-493d-9db6-53347cd848c4.png)
![image](https://user-images.githubusercontent.com/104628789/173783542-208c0af5-d97a-4ada-bf26-ea477eea01f7.png)
## PART II. Customer Clustering

- Criteria

![image](https://user-images.githubusercontent.com/104628789/173783722-035b826f-0506-4f43-b934-13d55921ceb9.png)
![image](https://user-images.githubusercontent.com/104628789/173783905-0adac6db-cc60-4ed0-9a73-f235f21d7d3b.png)

## PART III. Customer Purchase & Customer Lifetime Value Prediction
I applied for three model to preict Customer purchase in next 30 days from "lifetims library" with following model,
1. Beta Geometric Negative Binomial distribution (BG/NBD)
2. Modified Beta Geometric Negative Binomial Distribution (MBG/NBD)
3. Pareto Negative Binomial Distribution (Pareto NBD)
and then, combined the output of these model with "GammaGammaDistribution" to construct "Customer Lifetime Value Prediction"

### Results
![image](https://user-images.githubusercontent.com/104628789/173785337-19ab1565-6e03-45bb-adb4-47b12b1e18be.png)

![image](https://user-images.githubusercontent.com/104628789/173785409-ad28db21-7c2b-4693-971b-498b706031a3.png)

