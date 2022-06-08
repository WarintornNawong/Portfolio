# Stock Trading with RL Algorithm
## Introduction
### DATASET
I used the data from yahoo finance (yfinance offers a threaded and Pythonic way to download market data from Yahoo!Ⓡ finance.) to track the price history of "Games Stop Corporation" during 16 March 2020 to 12 March 2021.
**GameStop Corp.** is an American video game, consumer electronics, and gaming merchandise retailer.The company is headquartered in Grapevine, Texas (a suburb of Dallas), and is the largest video game retailer worldwide

## Part I : Exploratory Data Analysis

- Price & Volume History
![image](https://user-images.githubusercontent.com/104628789/171366842-4b11a53c-dd05-441f-a325-3737015ba6ad.png)

- Key Technical Analysis
![image](https://user-images.githubusercontent.com/104628789/171368225-57c1690c-b3f4-45cb-b5f8-77e829634855.png)

#### Key Definition
1. **Simple Moving Average (SMA)** : arithmetic moving average calculated by adding recent prices and then dividing that figure by the number of time periods in the calculation average.
2. **The relative strength index (RSI)** : a momentum indicator used in technical analysis that measures the magnitude of recent price changes to evaluate overbought or oversold conditions in the price of a stock or other asset.
3. **On Balance Volume (OBV)** : measures buying and selling pressure as a cumulative indicator that adds volume on up days and subtracts volume on down days.


- **Observation**

  - GameStop Corp. started the year trading around $19.00 a share as recently as August 2020. Yet, by the end of January, GameStop’s shares were trading at over $300, at one point hitting a high of $483. Experts raced to explain what happened - a band of individual traders against Wall Street hedge funds that were betting against GameStop’s success. The fact that many of these retail traders utilized a brokerage app named Robinhood only added to the narrative.
  - RSI, OBV is relative to the price of GameStop Corp, especially in the final transaction of the end of year 2021.

## Part II : Environment Creation 
To build the trading environment, I used the "gym-anytrading" library to apply RL algorithm to beat the Game Stop Corp trading.


## Part III : Algorithm Training
Three algorithm from "Stable Baseline-3" library was used to participate in trading environment which is specifeid below,
- Advantage Actor Critic (A2C)
- Deep Q Network (DQN)
- Proximal Policy Optimization (PPO)

## Results 
Test period : 01 April - 01 October 2020. 
### The Trading Strategy of General Information (OHLCV)
- Advantage Actor Critic (A2C)
![image](https://user-images.githubusercontent.com/104628789/171371006-54918304-bc8e-44b0-a29b-5ad3928b5671.png)


- Deep Q Network (DQN)
![image](https://user-images.githubusercontent.com/104628789/171371065-e1e42a75-f66c-4fe2-b305-0edfd39b02ad.png)

- Proximal Policy Optimization (PPO)
![image](https://user-images.githubusercontent.com/104628789/171371123-1675ffc2-53eb-427c-b85f-ae536c7a403b.png)

### The Trading Strategy of General Information (OHLCV) + Technical Analysis.
- Advantage Actor Critic (A2C)
![image](https://user-images.githubusercontent.com/104628789/171371183-b224cd69-6d64-46cc-9c2a-8c1652c60af3.png)


- Deep Q Network (DQN)
![image](https://user-images.githubusercontent.com/104628789/171371239-84a52c63-81a4-4635-81b5-b447ba07cec2.png)


- Proximal Policy Optimization (PPO)
![image](https://user-images.githubusercontent.com/104628789/171371313-61327d0a-8e70-4812-9021-282d999e2670.png)

### Final Return of all algorithm
![image](https://user-images.githubusercontent.com/104628789/171370819-0a911fd0-78e6-42e5-aa76-fd9db4b3bfdb.png)

### Conclusion
the learned A2C algorithm could beat the best return among the algorithm in the trading during "April to October 2020" with 400 % return.  

## Notebook
you can find notebook [here](https://github.com/WarintornNawong/Portfolio/blob/main/Stock%20Trading%20with%20RL%20Algorithm/Stock%20Trading%20with%20RL%20Algorithm.ipynb)

