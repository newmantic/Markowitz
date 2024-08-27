# Markowitz

The Markowitz Mean-Variance Optimization model, developed by Harry Markowitz in 1952, is a mathematical framework for constructing an investment portfolio that optimizes the trade-off between risk and return. The model helps investors find the portfolio that offers the highest expected return for a given level of risk or, equivalently, the lowest risk for a given level of expected return.


Expected Return (E(R_p)): The expected return of a portfolio is the weighted average of the expected returns of the individual assets within the portfolio.
E(R_p) = w_1 * E(R_1) + w_2 * E(R_2) + ... + w_n * E(R_n)
       = ∑ (w_i * E(R_i))
Where:
E(R_p) is the expected return of the portfolio.
w_i is the weight of asset i in the portfolio.
E(R_i) is the expected return of asset i.
n is the total number of assets in the portfolio.

Portfolio Variance (Var(R_p)): The variance of the portfolio return is a measure of the total risk of the portfolio. It accounts for the variances of individual asset returns and the covariances between them.
Var(R_p) = ∑ ∑ (w_i * w_j * Cov(R_i, R_j))
Where:
Var(R_p) is the variance of the portfolio return.
Cov(R_i, R_j) is the covariance between the returns of asset i and asset j.
w_i and w_j are the weights of assets i and j in the portfolio.

Covariance (Cov(R_i, R_j)): Covariance measures how two assets move together. If the covariance is positive, the assets tend to move in the same direction. If it is negative, they tend to move in opposite directions.
Cov(R_i, R_j) = E[(R_i - E(R_i)) * (R_j - E(R_j))]

Efficient Frontier: The efficient frontier is a set of optimal portfolios that offer the highest expected return for a given level of risk (or the lowest risk for a given level of return). Portfolios that lie on the efficient frontier are considered to be optimally balanced in terms of risk and return.

Optimization Problem: The optimization problem can be framed in two equivalent ways:

Minimize Risk for a Given Return:
min Var(R_p) 
subject to E(R_p) = target return

Maximize Return for a Given Risk:
max E(R_p)
subject to Var(R_p) = target risk



Estimate Expected Returns and Covariances:
Calculate the expected return E(R_i) for each asset.
Calculate the covariance matrix Cov(R_i, R_j) for the asset returns.

Construct the Portfolio:
Determine the weights w_i of each asset in the portfolio that minimize the portfolio variance Var(R_p) for a given target return E(R_p).

Optimize the Portfolio:
Use quadratic programming or other optimization techniques to find the portfolio weights that either minimize risk for a given level of return or maximize return for a given level of risk.

Plot the Efficient Frontier:
The efficient frontier is plotted by varying the target return E(R_p) and finding the corresponding minimum variance Var(R_p) for each level of return.
