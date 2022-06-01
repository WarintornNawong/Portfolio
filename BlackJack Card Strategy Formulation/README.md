## BlackJack Card Strategy Formulation
### Introduction
#### Dataset : 
"BlackJack Environment" from "Open AI Gym". Blackjack is a card game where the goal is to beat the dealer by obtaining cards that sum to closer to 21 (without going over 21) than the dealers cards.
- **Description** Face cards (Jack, Queen, King) have a point value of 10. Aces can either count as 11 (called a ‘usable ace’) or 1. Numerical cards (2-9) have a value equal to their number.This game is played with an infinite deck (or with replacement). The game starts with the dealer having one face up and one face down card, while the player has two face up cards. The player can request additional cards **(hit, action=1)** until they decide to stop **(stick, action=0)** or exceed 21 (bust, immediate loss). After the player sticks, the dealer reveals their facedown card, and draws until their sum is 17 or greater. If the dealer goes bust, the player wins. If neither the player nor the dealer busts, the outcome (win, lose, draw) is decided by whose sum is closer to 21
- **Action Space** : Discrete(2) - There are two actions: stick (0), and hit (1). 
- **Observation Space** : Tuple(Discrete(32), Discrete(11), Discrete(2)) - The observation consists of a 3-tuple containing: the player’s current sum, the value of the dealer’s one showing card (1-10 where 1 is ace), and whether the player holds a usable ace (0 or 1).
- **Rewards** : win game: +1, lose game: -1, draw game: 0

## PART I : Agent Development
To play the discrete problem in both action and observation space, the compatible algorithm I used is specified below,
- Q-Learning
- SARSA
- Expected-SARSA
- Monte Carlo Exploring Start
- Monte Carlo Control


## State-Value Function
### Q-Learning
![image](https://user-images.githubusercontent.com/104628789/171457168-2fe8076e-a48f-45ee-86fa-c0d397a9becf.png)
### SARSA
![image](https://user-images.githubusercontent.com/104628789/171457701-247e84aa-4df3-42ed-aa56-b19a0a0c40fc.png)
### Expected-SARSA



