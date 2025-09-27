# Estimating-Amazon-Stock-Option-Value-with-Python
This repository contains a Jupyter Notebook for estimating call option values on Amazon (AMZN) closing prices from 2024-01-02 to 2025-09-26 and using Monte Carlo simulation and the Black-Scholes formula. 

## Overview

This project estimates the value of a call option for Amazon stock with a strike price 5% above the current closing price ($219.78) and 21 days (1 month) to expiration.
- Monte Carlo simulation: For risk-neutral pricing and confidence intervals.
- Black-Sholes formula: For analytical validation.

Data: Historical closing prices from 'amazon_stock_data.csv'

## Key Concepts
- Volatility calculation: Annualized standard deviation of log returns.
- Monte Carlo simulation: Simulated stock paths using Geometric Brownian
- Black-Scholes formula:

<img width="633" height="360" alt="Image" src="https://github.com/user-attachments/assets/e336f2a8-559b-4fce-ae9d-7ee0596acb1c" />

    Run cells sequentially. Key parameters:
    - Current price: $219.78
    - Strike: $219.78 * 1.05 ≈ $230.77
    - Volatility: 26.81%
    - Risk-free rate: 5%
    - Time to expiration: 21 days
    - Simulations: 50,000

## Results

    - Estimated stock price after 21 days: $220.56 (mean)
    - Monte Carlo Call Option Price: $3.03 ± $0.03 (95% CI: $2.96–$3.09)
    - Black-Scholes Call Option Price: $3.05
    - Breakeven: $233.80 (strike + premium)
    
    Interpretation: The option is priced at ~$3.03–$3.05, with expected slight stock growth.

## Visualizations

Amazon Closing Prices (2024–2025):

<img width="850" height="518" alt="Image" src="https://github.com/user-attachments/assets/d504d67e-d812-4444-bb62-9d32fca2a574" />

Histogram of Simulated Ending Prices:

<img width="866" height="545" alt="Image" src="https://github.com/user-attachments/assets/c752cbf5-5c6e-4dcb-9f4b-9737ee153d1b" />

## Contact

- Thanh Xuyen Nguyen  
- LinkedIn: [xuyen-thanh-nguyen-0518](https://www.linkedin.com/in/xuyen-thanh-nguyen-0518/)  
- Email: thanhxuyen.nguyen@outlook.com
