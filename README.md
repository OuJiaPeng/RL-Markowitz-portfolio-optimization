## RL and Markowitz Portfolio Optimization
This project compares Markowitz and Reinforcement Learning based portfolio optimization.

More details can be found in the **"Project_slides.pdf"**

Overall, there are many aspects of this which could be improved on. Working towards a better solution [here](https://github.com/OuJiaPeng/Portfolio-Optimization).

- need to consider drawdown, turnover, and slippage
- model could use a lot more complexity and factor input
- just a plethora of issues, will be fixed in new project.

---

## Features
- **Classical Markowitz Optimization:** aimed to maximize Sharpe Ratio  
- **Deep Reinforcement Learning (PPO) Agent:** dynamic Portfolio Allocation, reward is Sharpe based  
- **Performance Comparison:** Markowitz, RL, and a Naive (equal weights) portfolio  
- **Visualizations:** Portfolio Weights and Wealth Growth  

---

## Project Structure

    RL-Markowitz-portfolio-optimization/  
    ├── RL_PPO/                              # Reinforcement Learning (PPO) Module  
    │   ├── RL_portfolio.py                  # Training Script  
    │   ├── evaluate_RL_portfolio.py         # Evaluation Script  
    │   ├── RL_average_weights_pie.png       # Results (Visuals & Metrics)  
    │   ├── RL_weights_over_time.png  
    │   ├── RL_wealth_growth.png  
    │   ├── RL_evaluation_summary.txt  
    │   └── ppo_portfolio_model_sharpe.zip   # Saved Model  
    │
    ├── markowitz/                           # Markowitz Optimization Module  
    │   ├── markowitz_portfolio.ipynb        # Jupyter Notebook for Markowitz  
    │   ├── markowitz_allocations_pie.png    # Results (Visuals & Metrics)  
    │   ├── markowitz_wealth_growth.png  
    │   └── markowitz_evaluation_metrics.txt 
    │  
    ├── naive/                               # Naive (Baseline) Portfolio  
    │   ├── naive_portfolio_plot.png         # Results (Visuals & Metrics)  
    │   └── naive_metrics.txt         
    │  
    ├── README.md                            # Project Overview and Guide  
    ├── requirements.txt                     # Dependency List  
    └── .gitignore                           # Git Ignore File  

---

## Results

| Portfolio         | Annualized Return | Volatility | Sharpe Ratio |
|------------------|-------------------|------------|--------------|
| Naive (Equal Wt) | 15.00%            | 10.70%     | 1.40         |
| Markowitz        | 25.37%            | 10.76%     | 2.36         |
| RL (PPO Agent)   | 18.99%            | 10.52%     | 1.81         |

Very surprised Markowitz performed this well — it feels like doing the wrong steps and getting the right answer on a test.

---

## Future Improvements

- Add transaction costs and turnover penalties

- Better optimize PPO hyperparameters

- Incorporate complexities for RL model

---

