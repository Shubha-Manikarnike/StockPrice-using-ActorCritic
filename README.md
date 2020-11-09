# StockPrice-using-ActorCritic
Apply the Q - Actor Critic on a StockPrice Problem

The data used for this problem is the Standard and Poor's 500 downloaded from Yahoo Finance
The train Data is from 2006 to 2015 and test Data is from 2015 to 2018.

The Actor Critic Solution helps us take 3 actions based on the Stock Price
  
  Hold
  Sell
  Buy

The Actor is the policy based model : which takes in the Stock Price and gives out a probability distribution for Hold, Buy or Sell
The Critic is a DQN which takes in the Stock Price and an Action given by the Actor and computes the Q value
Critic is trained to maximize the Q Value
The Q Value is used by the Actor to Improve probabilities of better actions

Below are the Update equations of the Actor and the Critic. For the Actor, the gradient is computed as Log Policy ( Log probability of the Actions ) times the Reward.
The reward is replaced with the Q-Value which is Computed by the Critic.
[Update Equations](https://github.com/Shubha-Manikarnike/StockPrice-using-ActorCritic/blob/main/Images/Q-ActorCritic.PNG)

Below is a snippet of the Q-Actor Critic

[Algorithm](https://github.com/Shubha-Manikarnike/StockPrice-using-ActorCritic/blob/main/Images/Q-ActoCritic%20Algorithm.PNG)
