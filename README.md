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
    ├── RL PPO/                                # Reinforcement Learning (PPO) Module
    │   ├── RL portfolio.py                    # PPO training script
    │   ├── evaluate RL portfolio.py           # PPO evaluation script
    │   ├── RL_average_weights_pie.png         # Portfolio weights (average) visualization
    │   ├── RL_evaluation_summary.txt          # Sharpe, return, volatility summary
    │   ├── RL_wealth_growth.png               # Portfolio wealth over time (PPO)
    │   ├── RL_weights_over_time.png           # Weights timeline (PPO)
    │   └── ppo_portfolio_model_sharpe.zip     # Trained PPO model
    │
    ├── markowitz/                             # Classic Markowitz Optimization Module
    │   ├── markowitz portfolio.ipynb          # Full implementation in notebook
    │   ├── corr_matrix_etf_train_returns.png  # Correlation heatmap of training set
    │   ├── markowitz_allocations_pie.png      # Portfolio weights (Markowitz)
    │   ├── markowitz_evaluation_metrics.txt   # Sharpe, return, volatility summary
    │   └── markowitz_wealth_growth.png        # Portfolio wealth over time (Markowitz)
    │
    ├── naive/                                 # Baseline Equal Weight Portfolio
    │   ├── naive portfolio.ipynb              # Naive equal-weight implementation
    │   ├── naive_metrics.txt                  # Evaluation metrics (return, Sharpe)
    │   └── naive_portfolio_plot.png           # Wealth growth plot (Naive)
    │
    ├── Project_slides.pdf                     # Presentation summary of project
    ├── README.md                              # Project overview and documentation
    ├── requirements.txt                       # Dependencies

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

