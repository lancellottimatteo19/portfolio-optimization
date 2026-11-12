# Portfolio Optimisation with CVXPY

Convex portfolio optimisation in the Markowitz mean-variance framework, with realistic constraints: no short
selling and a cap on the weight of each asset.

## Contents — [`efficient_frontier.ipynb`](efficient_frontier.ipynb)

* **Global minimum-variance (GMV)** portfolio with `CVXPY`.
* **Efficient frontier** with a concentration limit $w_i \le 0.35$ and no short selling.
* **Tangency portfolio** (maximum Sharpe ratio) through the **Charnes-Cooper** transformation, which turns the
  non-convex Sharpe maximisation into a convex quadratic programme, and the **Capital Market Line**.

## Results

With five synthetic assets and a 2% risk-free rate, the tangency portfolio has an expected return of 10.74%, a
volatility of 6.42% and a Sharpe ratio of 1.360; the GMV portfolio has an expected return of 9.74% and a volatility
of 6.10%.

## How to run

Requires Python 3.9 or later.

```bash
git clone https://github.com/lancellottimatteo19/portfolio-optimization-cvxpy.git
cd portfolio-optimization-cvxpy
pip install -r requirements.txt
jupyter lab
```

The notebook is saved with its outputs, so charts and results are visible directly on GitHub.
