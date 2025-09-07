# Monte Carlo Simulation Project

🎯 **Overview**

This project demonstrates the power and importance of Monte Carlo simulation across three domains:

- **π Estimation** – a simple geometric demo to build intuition.
- **European Call Option Pricing** – an application in financial engineering.
- **Portfolio Value at Risk (VaR)** – a risk management case study.

Monte Carlo is a universal tool: when uncertainty and complexity make closed-form solutions impossible, sampling scenarios provides reliable estimates.

---

📂 **Project Structure**
```text
monte_carlo_simulation/
│── monte_carlo_pi.ipynb      # Notebook for π estimation
│── option_pricing.ipynb      # Notebook for option pricing
│── Prtfolio_VaR.ipynb        # Notebook for VaR
│── README.md                 # Project documentation
```

---

🧩 **Simulations**

**1. Estimating π**
- Drop random points in a square.
- Count fraction that land in the inscribed circle.
- π ≈ 4 × (inside points / total points).

*Outputs:*
- Scatter plot of sampled points.
- Convergence plot showing π estimate approaching the true value.

**2. European Call Option Pricing**
- Model stock price with Geometric Brownian Motion (GBM).
- Simulate thousands of terminal stock prices.
- Payoff = max(S_T – K, 0).
- Discount to present → estimate option price.

*Outputs:*
- Option price estimate with 95% CI.
- Histogram of discounted payoffs.

**3. Portfolio Risk (VaR)**
- Assume 2-asset portfolio with given mean returns + covariance.
- Generate correlated returns with Cholesky decomposition.
- Simulate portfolio returns distribution.
- Compute Value at Risk (VaR) at 95% confidence.

*Outputs:*
- Histogram of portfolio returns with VaR marker.
- Summary statistics: mean, std, VaR.

---

📊 **Key Takeaways**
- Accuracy improves with more samples (error decreases ∝ 1/√N).
- Monte Carlo is flexible: it works with any distribution or model.
- Visualizations make uncertainty tangible for decision-making.
- Applications range from pure math → finance → risk management.

---

⚙️ **Requirements**
- Python 3.8+
- NumPy
- Matplotlib
- Pandas (for VaR)
- Jupyter Notebook

Install dependencies:
```bash
pip install numpy matplotlib pandas jupyter
```

---

🚀 **How to Run**
1. Clone this project.
2. Open Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
3. Run each notebook (`monte_carlo_pi.ipynb`, etc.).

---

📌 **License**

This project is open-source for learning and demonstration purposes.
