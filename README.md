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
