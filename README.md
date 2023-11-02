# Stock-Price-Prediction-with-Optimal-Portfolio-Allocation

## Problem Statement 
<p>To design a reinforcement learning based financial model that helps in deciding trading strategies for multiple stock trading in order to obtain maximum portfolio value based on current and the current position (vt = ct + x0pt) using attributes such as open, close, high, low and other Technical indicators such as date, tic, operating margin, net profit margin, return over assets, return on equity, earnings per share, book per share etc. Here, vt is total portfolio value,  ct is the current available cash and x0pt represents current position. Our aim is to maximize the total portfolio value vt by selecting the efficient trading strategies.</p>

## Proposed Solution
<p>We model the stock trading process as a Markov Decision Process (MDP) which consist of:<br><br>
  1. Action Space: Denoted as  {−k, …, −1, 0, 1, …, k}, where k denotes the number of shares. For 30 stocks the entire action space is (2k+1)*30.<br><br>
  2. State Space: Using 17 state space such as current ratio, quick ratio, cash ratio, inventory turnover, receivable turnover, payable turnover etc. (30 * 17 + 1).<br><br>
  3. Reward Function:  Derived by formula: (Portfolio Value at stock’s close price - Portfolio Value at stock’s open price)<br><br>
  4. Environment: multiple stock trading for Dow 30.<br><br>
</p>

## References
FinRL Architecture Description - https://finrl.readthedocs.io/en/latest/start/three_layer/environments.html<br>

https://openreview.net/forum?id=82nKnFErXUh<br>

https://www.wikipedia.com<br>

Matthew F. Dixon Igor Halperin Paul Bilokon - Machine Learning in Finance: From Theory to Practice <br>
