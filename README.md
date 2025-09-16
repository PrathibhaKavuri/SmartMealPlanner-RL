# **Smart Meal Planning with Reinforcement Learning**

This project applies RL to recommend products for ingredients,optimizing for both **budget** and **personal preferences**.Supermarkets offer multiple product options for each ingredient and finding the best combination manually can be overwhelming.The model automates this decision-making process.

The core approach uses a **Monte Carlo RL model**:  
- Ingredients are treated as **states**,products as **actions**.  
- Each episode simulates selecting products for all ingredients at once.  
- After each episode.. the total cost is checked against the budget and rewards guide future selections.  

The model balances **exploration and exploitation** occasionally trying new combinations but mainly selecting the best-known options.Over time it converges to combinations that satisfy budget constraints while favoring better products.

Key points:  
- Evaluates long-term value of product choices rather than immediate outcomes.  
- Can scale to larger datasets with more ingredients and products.  
- Allows tuning of hyperparameters like learning rate,exploration rate and budget.  

It also helps understand the trade-offs between cost and quality making the decision process more intuitive and data-driven.
