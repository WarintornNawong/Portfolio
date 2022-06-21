## Airline Tweet Sentiment Prediction
### Introduction
#### Dataset
A sentiment analysis job about the problems of each major U.S. airline. Twitter data was scraped from February of 2015 and contributors were asked to first classify positive, negative, and neutral tweets, followed by categorizing negative reasons (such as "late flight" or "rude service"). You can download the non-aggregated results (55,000 rows) here.
### Part I. Exploratory Data Analysis
- Airline Sentiment by U.S. Airline company
![image](https://user-images.githubusercontent.com/104628789/172572044-7b4fb199-1a90-4868-9dc9-541ab72ed5f3.png)
- Sentiment by Topic
![image](https://user-images.githubusercontent.com/104628789/172572171-755b85a8-434c-4a30-8adc-2f74ce9458f5.png)
![image](https://user-images.githubusercontent.com/104628789/172572278-f44b5a7e-3811-4db0-84fc-be943005ec9c.png)
![image](https://user-images.githubusercontent.com/104628789/172572541-dc28d391-3b27-4bd5-9290-b906e8d3061b.png)
![image](https://user-images.githubusercontent.com/104628789/172572584-e9b17345-469d-4155-a401-a1680247f63e.png)
![image](https://user-images.githubusercontent.com/104628789/172572657-29bf5412-c1eb-4691-895d-786b8956072a.png)
![image](https://user-images.githubusercontent.com/104628789/172572873-ebeafa55-db3f-4b8d-9433-5eb361983da9.png)
![image](https://user-images.githubusercontent.com/104628789/172572910-fb02eda0-662c-4ec8-80ad-abe13c20a4c4.png)
![image](https://user-images.githubusercontent.com/104628789/172572959-051faea3-a360-4ab8-b3f8-dc5b33b513b9.png)
![image](https://user-images.githubusercontent.com/104628789/172573003-abe016f4-288d-47ce-8f04-7eb699ef94b5.png)
![image](https://user-images.githubusercontent.com/104628789/172573054-cdb31200-c040-4f87-8ff7-4151ad2117bc.png)

### Observation
United Airline ranked first in high negative sentiment tweet, followed by U.S. Airways and American Airline. The n-gram methods in second, thirdth and fourth consist of **"Flight Cancellation and delay"**.The pattern of negative tweets is summarizable in the following details,
1. Longer character
2. Higher word count
3. Higher Punctuation
4. Higher stopwords

## Part II. Text Processing
Before developing model, I applied the step of cleaning & Preprocssing with the following details,

1.Remove airline

2.Remove url

3.Remove HTML Tags

4.Expand Contraction

5.lowercase 

6.Remove repeated character

7.Remove Number

8.Remove puntuation    

9.Remove STOPWORDS

10.Remove Whitespace

11.Convert to lemmatized word

## PART III. Model Construction

I selected the classification model from ensemble-based algorithm and embedding deep learning with following model,
1. RandomForest
2. GradientBoosting
3. AdaBoost
4. XGBoost
5. Long Short-Term Memory (LSTM)

to test in four case
- Baseline without Undersampling process.
- Baseline with Undersampling process
- Hyperparameter tuning without Undersampling process
- Hyperparameter tuning with Undersampling process.

## PART IV. Results

the best model is "RandomForest in base model without hyperparameter tuning and undersampling process"
![image](https://user-images.githubusercontent.com/104628789/172577851-b1bf73ab-284a-47fb-94cc-3cbc93ae4a20.png)

## Notebook
you can find notebook [here](https://github.com/WarintornNawong/Portfolio/blob/main/Airline%20Tweet%20Sentiment%20Prediction/US%20Airline%20Tweet%20Sentiment%20Analysis.ipynb)
