# Telco Customer Churn Prediction
## Introduction
### DATASET
The Telco customer churn data contains information about a fictional telco company that provided home phone and Internet services to 7043 customers in California in Q3. It indicates which customers have left, stayed, or signed up for their service. Multiple important demographics are included for each customer, as well as a Satisfaction Score, Churn Score. you can find data [here](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

#### ***DEMOGRAPHICS***



**CustomerID**: A unique ID that identifies each customer.

**Gender**: The customer’s gender: Male, Female

**Senior Citizen**: Indicates if the customer is 65 or older: Yes, No

**Partner** : Whether the customer has a partner or not Yes, No

**Dependents**: Indicates if the customer lives with any dependents: Yes, No. Dependents could be children, parents, grandparents, etc



#### ***SERVICES***

- **Tenure**: Indicates the total amount of months that the customer has been with the company by the end of the quarter specified above.

- **Phone Service**: Indicates if the customer subscribes to home phone service with the company: Yes, No

- **Multiple Lines**: Indicates if the customer subscribes to multiple telephone lines with the company: Yes, No

- **Internet Service**: Indicates if the customer subscribes to Internet service with the company: No, DSL (Digital Subscriber Line), Fiber Optic, Cable.

- **Online Security**: Indicates if the customer subscribes to an additional online security service provided by the company: Yes, No

- **Online Backup**: Indicates if the customer subscribes to an additional online backup service provided by the company: Yes, No

- **Device Protection** : Indicates if the customer subscribes to an additional device protection plan for their Internet equipment provided by the company: Yes, No

- **Tech Support**: Indicates if the customer subscribes to an additional technical support plan from the company with reduced wait times: Yes, No

- **Streaming TV**: Indicates if the customer uses their Internet service to stream television programing from a third party provider: Yes, No. The company does not charge an additional fee for this service.

- **Streaming Movies**: Indicates if the customer uses their Internet service to stream movies from a third party provider: Yes, No. The company does not charge an additional fee for this service.

- **Contract**: Indicates the customer’s current contract type: Month-to-Month, One Year, Two Year.

- **Paperless Billing**: Indicates if the customer has chosen paperless billing: Yes, No

- **Payment Method**: Indicates how the customer pays their bill: Bank Withdrawal, Credit Card, Mailed Check

- **Monthly Charge**: Indicates the customer’s current total monthly charge for all their services from the company.

- **Total Charges**: Indicates the customer’s total charges, calculated to the end of the quarter specified above.

## Key Findings

### Monthly Chrage and Tenure per attribute

![image](https://user-images.githubusercontent.com/104628789/170277795-390f1468-d454-47b2-a7d6-e770d561eee1.png)
![image](https://user-images.githubusercontent.com/104628789/170277890-dc7d83ec-1724-492d-912a-6918c715bf18.png)
![image](https://user-images.githubusercontent.com/104628789/170278011-d8f6ede4-4205-4fe3-aabf-597f4b563eb2.png)
![image](https://user-images.githubusercontent.com/104628789/170278090-ef0db138-4573-47d2-8184-4ed6e7d62a56.png)
![image](https://user-images.githubusercontent.com/104628789/170278179-486a6b20-8f77-4e04-943b-96a33f53c7af.png)
![image](https://user-images.githubusercontent.com/104628789/170278238-7768ddfd-f28a-43d8-bccb-9e88f669422e.png)
![image](https://user-images.githubusercontent.com/104628789/170278294-3bbeb799-3f53-45a7-9b7a-2afc05d1a872.png)
![image](https://user-images.githubusercontent.com/104628789/170278357-bf9664f4-27c0-45dc-9a1d-b891c9708249.png)
![image](https://user-images.githubusercontent.com/104628789/170278419-b6d12bfc-af0e-4e6e-823c-5c648485169a.png)
![image](https://user-images.githubusercontent.com/104628789/170278503-562c23cb-be3d-4080-afbd-49588a3b87d0.png)
![image](https://user-images.githubusercontent.com/104628789/170278599-9397a4ba-cfd3-43f6-a8dd-1e5ad877603e.png)
![image](https://user-images.githubusercontent.com/104628789/170278631-ffa9340c-17ce-4124-8a95-7c91309c0eb1.png)
![image](https://user-images.githubusercontent.com/104628789/170278684-7ed01639-214e-46db-88c8-cce3d414517c.png)
![image](https://user-images.githubusercontent.com/104628789/170278767-f9110cdd-0b7b-41cc-842c-3a26cc6c971c.png)
![image](https://user-images.githubusercontent.com/104628789/170278821-a419a802-f4a4-4321-be60-c6aadfa6350e.png)
![image](https://user-images.githubusercontent.com/104628789/170278860-369ba101-8ef7-4d90-aeb1-3faf62006a55.png)

### First Observation
the most of churn customer always have less tenure period on almost every attribute such as Contract Type, Streaming or online Security Services etc. one of attribute that have less different in monthly charge and tenure is gerder. so it can be concluded that likelihood of churn is not relevant to gender. Moreover, they indicates that Contract type have higher charge for churn customer than non-churn.

## #### Probability of Churn and Retention per attribute
![image](https://user-images.githubusercontent.com/104628789/170279890-f7dadc57-5d8b-4a0d-9b8a-0d4b95bb1ac7.png)
![image](https://user-images.githubusercontent.com/104628789/170279947-d07c92d7-b003-44f9-b9e8-e012b9442f0a.png)
![image](https://user-images.githubusercontent.com/104628789/170279998-8832b6ca-9742-42a5-94e5-e8c154c95b4b.png)
![image](https://user-images.githubusercontent.com/104628789/170280052-e6297693-437e-4b0f-bf65-4438dad45c8c.png)
![image](https://user-images.githubusercontent.com/104628789/170280096-f9b72bd8-ce47-4fdb-bbd9-95deaa7a7d0a.png)
![image](https://user-images.githubusercontent.com/104628789/170280139-2a401723-17e1-4610-92ab-12f110a49a50.png)
![image](https://user-images.githubusercontent.com/104628789/170280226-7daf46eb-d081-4d47-923f-21e419a1f60f.png)
![image](https://user-images.githubusercontent.com/104628789/170280424-2ad99c74-752c-4483-aa5f-08044690984e.png)
![image](https://user-images.githubusercontent.com/104628789/170280463-8db7a9ab-1582-4fde-a7bf-7b5547edb9a8.png)
![image](https://user-images.githubusercontent.com/104628789/170280500-bf64d780-1348-4dd9-82df-caa464f13b81.png)
![image](https://user-images.githubusercontent.com/104628789/170280537-8787b9ca-7f31-4302-a5be-6b5e2a1bf7ea.png)
![image](https://user-images.githubusercontent.com/104628789/170280574-cde93220-9add-41f6-b3ea-7ba76cf8b0ad.png)
![image](https://user-images.githubusercontent.com/104628789/170280734-aa8fff52-fe11-4074-a0ce-e624e4fa3d4b.png)
![image](https://user-images.githubusercontent.com/104628789/170280771-2b602dc7-7cc4-47af-86e9-29474e2eee1b.png)
![image](https://user-images.githubusercontent.com/104628789/170280800-d5de7a10-3fa6-44f3-80b9-9c0393b12bcc.png)
![image](https://user-images.githubusercontent.com/104628789/170280834-6da06f23-d6d1-439b-a70b-7cb31414ab0d.png)

### Second Observation
Fiber Optic in Internet Service, Phone Service, Tech Support, Electronics Check in Payment Method and Month-to-month contract tyoe contribute the significant churn probability than the rest of attribute.

## Model Construction
In this kind of data, churn prediction is a classification problem so I decided to select a classification algorithm through "Augluon algorithm" to find the group of high performing model to proceed fine-tuning. the selected algorithm for "Telco Churn Prediction" is specified below,

1. RandomForestClassifier (rf)
2. GradientBosstingClassifier (gb)
3. AdaBoosting (ada)
4. XGBoosting (xg)
5. LightBoosting (lgb)
6. CatBoosting (cbc)

![image](https://user-images.githubusercontent.com/104628789/170283915-c14703ee-f095-4160-8a75-af8d9853ab16.png)

The result show that the highest ROC-AUC score is "CatBoostClassifier" with 0.8329 score

## Feature Improtance
the key feature importance for each algorithm use to predict customer churn probability.
![image](https://user-images.githubusercontent.com/104628789/170284428-8617af96-0e32-41b9-8595-6d8b4860bb8a.png)
![image](https://user-images.githubusercontent.com/104628789/170284453-25a9bfdd-c355-49e2-808c-5804f5981e19.png)
![image](https://user-images.githubusercontent.com/104628789/170284480-030099d2-42f6-4534-b96f-7d2f584a7773.png)

### Combined Feature Importance

![image](https://user-images.githubusercontent.com/104628789/170284627-4c0c9f15-3295-497d-90a1-fcbabed63797.png)

the top 3 key feature importanfe after combination of all algorithm are "Contract type, tenure and payment method"












