# E-commerce Customer Segmentation and Customer Lifetime Value Prediction
## Introduction
In markerting task, the most concept before formulating any strategy is to "Know Your Customer (KYC)" to put the right strategy with the right people. Therefore, the history data would play major role to create and constructing the "Customer Segmentation" and and to build the customer lifetime value indicator to help personalization more effective.
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

## PART I. Exploratory Data Analysis
![image](https://user-images.githubusercontent.com/104628789/173783431-283a1b05-7c20-4868-9383-4e2ee779b6f5.png)
![image](https://user-images.githubusercontent.com/104628789/173783513-a65e696b-f90d-493d-9db6-53347cd848c4.png)
![image](https://user-images.githubusercontent.com/104628789/173783542-208c0af5-d97a-4ada-bf26-ea477eea01f7.png)

- **Observation** 
1. The end of the year is the most purchaesed period for purchusing with the high festival such as Christmas, New Year etc. 
2. 11 - 12 o'clock are the most purchased time during the day.
3. Thursday is the most purchased day of week in online customer.

## PART II. Customer Clustering

In order to segment customer, I start applying the criteria between frequency and monetary as F&M Criticality from converting "Invoice Data", "Customer ID" and "Revenue" to be " Standard Recency, Frequency and Monetary" and then apply the result with recency to obtain a customer class/segment in order to provide the segment-based strategy.

### Criteria for Customer Segmentation
![image](https://user-images.githubusercontent.com/104628789/173783722-035b826f-0506-4f43-b934-13d55921ceb9.png)

### Definition
1. **Champions**: Bought recently, buy often and spend the most
2. **Loyal customers**: Buy on a regular basis. Responsive to promotions.
3. **Potential loyalist**: Recent customers with average frequency.
4. **Recent customers**: Bought most recently, but not often.
5. **Promising**: Recent shoppers, but haven’t spent much.
6. **Needs attention**: Above average recency, frequency and monetary values. May not have bought very recently though.
7. **About to sleep**: Below average recency and frequency. Will lose them if not reactivated.
8. **At risk**: Some time since they’ve purchased. Need to bring them back!
9. **Can’t lose them**: Used to purchase frequently but haven’t returned for a long time.
10. **Hibernating**: Last purchase was long back and low number of orders. May be lost.

### Actionable strategy

1. **Champions**: Reward them. They can become evangelists and early adopters of new products.
2. **Loyal customers**: Up-sell higher value products. Engage them. Ask for reviews.
3. **Potential loyalist**: Recommend other products. Engage in loyalty programs.
4. **Recent/new customers**: Provide a good onboarding process. Start building the relationship.
5. **Promising**: Create more brand awareness. Provide free trials.
6. **Needs attention**: Reactivate them. Provide limited time offers. Recommend new products based on purchase history.
7. **About to sleep**: Reactivate them. Share valuable resources. Recommend popular products. Offer discounts.
8. **At risk**: Send personalised email or other messages to reconnect. Provide good offers and share valuable resources.
9. **Can’t lose them**: Win them back. Talk to them. Make them special offers. Make them feel valuable.
10. **Hibernating**:Recreate brand value. Offer relevant products and good offers.

### RFM Analysis for each segments.

![image](https://user-images.githubusercontent.com/104628789/173783905-0adac6db-cc60-4ed0-9a73-f235f21d7d3b.png)

- **Observation**
1. Can't loose, Champion and Loyal customer is the one who frequently and constantly contribute high value in online purchasing.
2. New Customer is who pay highest revenue among the rest of customer.

## PART III. Customer Purchase & Customer Lifetime Value Prediction
I applied for three model to preict Customer purchase in next 30 days from "lifetims library" with following model,
1. Beta Geometric Negative Binomial distribution (BG/NBD)
2. Modified Beta Geometric Negative Binomial Distribution (MBG/NBD)
3. Pareto Negative Binomial Distribution (Pareto NBD)
and then, combined the output of these model with "GammaGammaDistribution" to construct "Customer Lifetime Value Prediction"

## Results
### Purchased Prediction Error
![image](https://user-images.githubusercontent.com/104628789/173785337-19ab1565-6e03-45bb-adb4-47b12b1e18be.png)

The results of these error is similar in all model - NG/NBD, MBG/NBD and Pareto NBD with insignificant different. However, the least error is "Pareto/NBD Model"

### Predicted Customer Lifetime Value

Customer Lifetime Value is a prognostication of the net profit contributed to the whole future relationship with a customer.

![image](https://user-images.githubusercontent.com/104628789/173799231-5d98848d-667b-4ce0-ac03-701af7da3992.png)


![image](https://user-images.githubusercontent.com/104628789/173785409-ad28db21-7c2b-4693-971b-498b706031a3.png)

The "Can't Loose" Customer pay highest CLV among the rest of segments in every model, followed by Loyal Customer and At-Risk. These figure could supplement the important of these customer type to abide by the actionable strategy in order to maximize marketing campagin efficiency. 
