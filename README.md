## RL and Markowitz Portfolio Optimization
This project compares Markowitz and Reinforcement Learning based portfolio optimization.

More details can be found in the **"Project_slides.pdf"**

Overall, there are many aspects of this which could be improved on. Working towards a better solution [here](https://github.com/OuJiaPeng/Portfolio-Optimization).

- Need to consider drawdown, turnover, and slippage
- Model could use a lot more complexity and factor input
- Just a handful of issues, will be fixed in new project.

---

## Results

| Portfolio         | Annualized Return | Volatility | Sharpe Ratio |
|------------------|-------------------|------------|--------------|
| Naive (Equal Wt) | 15.00%            | 10.70%     | 1.40         |
| Markowitz        | 25.37%            | 10.76%     | 2.36         |
| RL (PPO Agent)   | 18.99%            | 10.52%     | 1.81         |

Very surprised Markowitz performed this well — it feels like doing the "wrong" steps and getting the right answer on a test.

---

## Features
- **Classical Markowitz Optimization:** aimed to maximize Sharpe Ratio  
- **Deep Reinforcement Learning (PPO) Agent:** dynamic Portfolio Allocation, reward is Sharpe based  
- **Performance Comparison:** Markowitz, RL, and a Naive (equal weights) portfolio  
- **Visualizations:** Portfolio Weights and Wealth Growth  

---

## Project Structure

    RL-Markowitz-portfolio-optimization/
    ├── RL PPO/                                # Reinforcement Learning (PPO) Module
    │   ├── RL portfolio.py
    │   ├── evaluate RL portfolio.py
    │   ├── RL_average_weights_pie.png
    │   ├── RL_evaluation_summary.txt
    │   ├── RL_wealth_growth.png
    │   ├── RL_weights_over_time.png
    │   └── ppo_portfolio_model_sharpe.zip
    │
    ├── markowitz/                             # Classic Markowitz Optimization Module
    │   ├── markowitz portfolio.ipynb
    │   ├── corr_matrix_etf_train_returns.png
    │   ├── markowitz_allocations_pie.png
    │   ├── markowitz_evaluation_metrics.txt
    │   └── markowitz_wealth_growth.png
    │
    ├── naive/                                 # Baseline Equal Weight Portfolio
    │   ├── naive portfolio.ipynb
    │   ├── naive_metrics.txt
    │   └── naive_portfolio_plot.png
    │
    ├── Project_slides.pdf                     # Presentation summary of project
    ├── README.md
    ├── requirements.txt

---

## Future Improvements

- Add transaction costs and turnover penalties

- Better optimize PPO hyperparameters

- Incorporate complexities for RL model

---

