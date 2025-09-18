```markdown
# Investments: Finance 2 - BFIN (Lecture 5)

## Outline
* Portfolio Theory and Practice I
  * Efficient Diversification

## Opportunity Set of Risky Assets
* Minimum-variance frontier shows the risk-return opportunities available to the investor.
* Efficient frontier
  * There is an efficient portfolio for each risk level.
  * Portfolios on the efficient frontier represent trade-offs in terms of risk and return.

| ΓΑ | 10.10% | rB | 9.40% | Cov(ΓΑ, ΓB) | -0.000414 |
|---|---|---|---|---|---|
| σΑ | 1.70% | σΒ | 2.54% | | |
| σΑ^2 | 0.000289 | σΒ^2 | 0.00064516 | | |

| WA | WB | rp | σp^2 | σp |
|---|---|---|---|---|
| 100% | 0% | 10.100% | 0.000289 | 1.70% |
| 90% | 10% | 10.030% | 0.000166 | 1.29% |
| 80% | 20% | 9.960% | 0.000078 | 0.88% |
| 70% | 30% | 9.890% | 0.000026 | 0.51% |
| 60% | 40% | 9.820% | 0.000009 | 0.29% |
| 50% | 50% | 9.750% | 0.000027 | 0.52% |
| 40% | 60% | 9.680% | 0.000080 | 0.89% |
| 30% | 70% | 9.610% | 0.000168 | 1.30% |
| 20% | 80% | 9.540% | 0.000292 | 1.71% |
| 10% | 90% | 9.470% | 0.000451 | 2.12% |
| 0% | 100% | 9.400% | 0.000645 | 2.54% |

## Opportunity Set of Risky Assets

| | Global MV Portfolios No Short | Global MV Portfolios With Short |
|---|---|---|
| AMD | 0.00% | -5.53% |
| AMZN | 9.39% | 12.12% |
| FORD | 0.00% | -4.49% |
| JPM | 2.79% | 7.59% |
| NVDA | 0.00% | 1.04% |
| PFE | 38.25% | 38.18% |
| TGT | 18.82% | 20.74% |
| XOM | 30.75% | 30.35% |
| E(rp) | 0.62% | 0.68% |
| σp | 4.41% | 4.31% |
| rf | 0.41% | 0.41% |
| Sharpe Ratio | 0.0480 | 0.0641 |

## Capital Allocation to Risk-free and Risky Assets
* Complete portfolio consists of the risky asset and the risk-free asset.
  * A portfolio risk closer to the desired level can be achieved by changing the weights of risk-free asset and risky assets in the complete portfolio.

$W_{rf} + W_{risky} = 1$
$W_{rf} = 1 - W_{risky}$
$E(r_p) = (1 - W_{risky}) \cdot r_f + W_{risky} \cdot E(r_{risky})$
$E(r_p) = r_f + W_{risky} \cdot [E(r_{risky}) - r_f]$
$\sigma^2(r_p) = w_{rf}^2 \cdot \sigma^2(r_f) + W_{risky}^2 \cdot \sigma^2(r_{risky}) + 2 \cdot W_{rf}W_{risky}Cov(r_f, r_{risky})$
Since $\sigma^2(r_f) = 0$ and $Cov(r_f, r_{risky}) = 0$,
$\sigma^2(r_p) = W_{risky}^2 \cdot \sigma^2(r_{risky})$

## Capital Allocation to Risk-free and Risky Assets
If $\sigma^2(r_p) = w_{risky}^2 \cdot \sigma^2(r_{risky})$ then $\sigma(r_p) = W_{risky} \cdot \sigma(r_{risky})$
Thus, $W_{risky} = \frac{\sigma(r_p)}{\sigma(r_{risky})}$
$E(r_p) = r_f + W_{risky} \cdot [E(r_{risky}) - r_f]$
$E(r_p) = r_f + \frac{\sigma(r_p)}{\sigma(r_{risky})} \cdot [E(r_{risky}) - r_f]$
$E(r_p) = r_f + \left[ \frac{E(r_{risky})-r_f}{\sigma(r_{risky})} \right] \cdot \sigma(r_p)$
**Capital Allocation Line**

## Capital Allocation to Risk-free and Risky Assets
* Suppose the risk-free interest rate is 5%, the expected return and the standard deviation of the risky portfolio are 12% and 15%, respectively. Then;
$E(r_p) = r_f + \left[ \frac{E(r_{risky}) - r_f}{\sigma(r_{risky})} \right] \cdot \sigma(r_p)$
$E(r_p) = 0.05 + \left[ \frac{0.12-0.05}{0.15} \right] \cdot \sigma(r_p)$
$E(r_p) = 0.05 + 0.4667 \cdot \sigma(r_p)$

## Opportunity Set of Risky Assets

| | Global MV Portfolios No Short | Global MV Portfolios With Short | Optimal Risk Portfolios No Short | Optimal Risk Portfolios With Short |
|---|---|---|---|---|
| AMD | 0.00% | -5.53% | 0.00% | -34.75% |
| AMZN | 9.39% | 12.12% | 43.48% | 70.83% |
| FORD | 0.00% | -4.49% | 0.00% | -58.61% |
| JPM | 2.79% | 7.59% | 11.42% | 80.15% |
| NVDA | 0.00% | 1.04% | 45.10% | 76.25% |
| PFE | 38.25% | 38.18% | 0.00% | -71.24% |
| TGT | 18.82% | 20.74% | 0.00% | 16.91% |
| XOM | 30.75% | 30.35% | 0.00% | 20.46% |
| E(rp) | 0.62% | 0.68% | 1.91% | 3.36% |
| σp | 4.41% | 4.31% | 9.38% | 14.09% |
| rf | 0.41% | 0.41% | 0.41% | 0.41% |
| Sharpe Ratio | 0.0480 | 0.0641 | 0.1600 | 0.2097 |

## Opportunity Set of Risky Assets

| | Global MV Portfolios No Short | Global MV Portfolios With Short | Optimal Risk Portfolios (Group 1) No Short | Optimal Risk Portfolios (Group 1) With Short | Optimal Risk Portfolios (Group 2) No Short | Optimal Risk Portfolios (Group 2) With Short |
|---|---|---|---|---|---|---|
| SP500 | | | 29.84% | 57.82% | 0.00% | -84.30% |
| NDQ100 | | | 0.00% | 13.84% | 0.00% | 147.04% |
| EEM | | | 0.00% | -21.19% | 0.00% | -81.67% |
| XAU | | | 41.40% | 42.21% | 36.33% | 67.76% |
| AMD | 0.00% | -5.53% | 0.00% | -5.36% | 0.00% | -14.61% |
| AMZN | 9.39% | 12.12% | 0.00% | -1.13% | 43.48% | 70.83% |
| FORD | 0.00% | -4.49% | 0.00% | -5.19% | 0.00% | -58.61% |
| JPM | 2.79% | 7.59% | 0.00% | 0.85% | 11.42% | 80.15% |
| NVDA | 0.00% | 1.04% | 0.00% | -1.72% | 45.10% | 76.25% |
| PFE | 38.25% | 38.18% | 13.72% | 8.34% | 0.00% | -71.24% |
| TGT | 18.82% | 20.74% | 5.43% | 3.88% | 0.00% | 16.91% |
| XOM | 30.75% | 30.35% | 9.60% | 7.64% | 0.00% | 20.46% |
| E(rp) | 0.62% | 0.68% | 0.65% | 0.77% | 1.91% | 3.36% |
| σp | 4.41% | 4.31% | 3.25% | 2.92% | 9.38% | 14.09% |
| rf | 0.41% | 0.41% | 0.41% | 0.41% | 0.41% | 0.41% |
| Sharpe Ratio | 0.0480 | 0.0641 | 0.0733 | 0.1231 | 0.1600 | 0.2097 | 0.1669 | 0.2644 |

## Opportunity Set of Risky Assets

## Capital Allocation to Risk-free and Risky Assets
* Each CAL is uniquely identified by its slope.
* The optimal risky portfolio is the tangency portfolio
  * The unique portfolio with the highest Sharpe-Ratio.
* The optimal risky portfolio does not involve the degree of risk aversion of any individual investor.
* Every investor, regardless of her/his level of risk aversion, will agree on the best CAL, and allocate her/his wealth between risk-free asset and the optimal risky portfolio.
* The portion invested in the optimal risky portfolio, however, will depend on each investor's degree of risk.

## Capital Allocation to Risk-free and Risky Assets

## The Opportunity Set with Different Borrowing and Lending Rates
$r_f=7\%$
$E(r_p) = 15\%$
$\sigma_{rf}= 0\%$
$\sigma_p = 22\%$

Lend at $r_f = 7\%$ and borrow at $r_f = 9\%$

Lending range slope = 8/22 = 0.36
Borrowing range slope = 6/22 = 0.27

## The Investment Decision
* Top-down process with 3 steps:
  * Capital allocation: risky portfolio and risk-free asset
  * Asset allocation: across broad asset classes
  * Security selection: individual assets within an asset class

## The Investment Decision
### The Opportunity Set of the Debt and Equity Funds
* Portfolio A: 82% in bonds and 18% in stocks
  * $E(r_A) = 8.9\%$
  * $\sigma_A = 11.45\%$
* Portfolio B: 70% in bonds and 30% in stocks
  * $E(r_B) = 9.5\%$
  * $\sigma_B = 11.70\%$
* Maximize the slope of the CAL for any possible portfolio, P
* The objective function is the slope:
$$S_P = \frac{E(r_p) - r_f}{\sigma_p}$$

## The Investment Decision
### The Opportunity Set of the Debt and Equity Funds
* Portfolio A
  * $E(r_A) = 8.9\%$
  * $\sigma_A = 11.45\%$
$$S_A = \frac{E(r_A) - r_f}{\sigma_A} = \frac{8.9\% - 5\%}{11.45\%} = 0.34$$
* Portfolio B
  * $E(r_B) = 9.5\%$
  * $\sigma_B = 11.70\%$
$$S_B = \frac{E(r_B) - r_f}{\sigma_B} = \frac{9.5\% - 5\%}{11.70\%} = 0.38$$

## The Investment Decision
### The Opportunity Set of the Debt and Equity Funds
**Optimal Risky Portfolio**
* $E(r_p) = 11\%$
* $\sigma_p = 14.2\%$
$$S_p = \frac{E(r_p) - r_f}{\sigma_p} = \frac{11\%-5\%}{14.2\%} = 0.42$$

## The Investment Decision

| | |
|---|---|
| Port Mean | 11.00% |
| Port Variance | 0.0202 |
| Port Std Dev | 14.20% |
| RF | 5.00% |
| Sharpe Ratio | 0.4226 |

| | Mean | StdDev |
|---|---|---|
| Bonds | 8.00% | 12.00% |
| Equity | 13.00% | 20.00% |

Correlation = 0.3
Weights: 40.00% (Bonds), 60.00% (Equity)

| Constraints | 1 | 1 | 1 |
|---|---|---|---|

**Portfolio Variance**
| | Bonds | Equity |
|---|---|---|
| 40.00% Bonds | 0.002304 | 0.001728 |
| 60.00% Equity | 0.001728 | 0.014400 |
| Total | 0.020160 | 0.004032 | 0.016128 |

**Covariance Matrix**
| | Bonds | Equity |
|---|---|---|
| Bonds | 0.014400 | 0.007200 |
| Equity | 0.007200 | 0.040000 |

$$E(r_p) = W_1 E(r_1) + W_2 E(r_2) + \dots + W_N E(r_N)$$
$$\sigma^2(r_p) = w_1^2 \cdot \sigma^2(r_1) + w_2^2 \cdot \sigma^2(r_2) + 2 \cdot W_1 W_2 Cov(r_1, r_2)$$
$$\rho_{i,j} = \frac{cov(r_i, r_j)}{\sigma_i \sigma_j}$$

## The Investment Decision

$$U = E(r) - \frac{1}{2} A \sigma^2$$
Expected return on the complete portfolio:
$E(r_c) = r_f + y[E(r_p) - r_f]$
$\sigma_c = y \times \sigma_p$
$$\max_y U = E(r_c) - \frac{1}{2} A \sigma_c^2$$
$$\max_y U = r_f + y[E(r_p) - r_f] - \frac{1}{2} A y^2 \sigma_p^2$$
$$y^* = \frac{E(r_p) - r_f}{A \sigma_p^2}$$
Optimal Allocation to P: A=4
$$y^* = \frac{11\%-5\%}{4 \times (14.2\%)^2} = 0.7439$$

## Markowitz Portfolio Optimization Model

## Markowitz Portfolio Optimization Model
* Security selection
  * Determine the risk-return opportunities available
  * All portfolios that lie on the minimum-variance frontier from the global minimum-variance portfolio and upward provide the best risk-return combinations
* Search for the CAL with the highest reward-to-variability ratio
  * Everyone invests in P, regardless of their degree of risk aversion
    * More risk-averse investors put less in P
    * Less risk-averse investors put more in P

## Markowitz Portfolio Optimization Model
* Capital Allocation and the Separation Property
  * The portfolio choice problem may be separated into two independent tasks
    * Determination of the optimal risky portfolio is purely technical
    * Allocation of the complete portfolio to risk-free versus the risky portfolio depends on personal preference

## Markowitz Portfolio Optimization Model
* Optimal Portfolios and Nonnormal Returns
  * Fat-tailed distributions can result in extreme values of VaR and ES.
  * If other portfolios provide sufficiently better VaR and ES values than the mean-variance efficient portfolio, we may prefer these when faced with fat-tailed distributions.

## Markowitz Portfolio Optimization Model
* Passive Strategies: The Capital Market Line
  * Determination of the assets to include in P may result from a passive or an active strategy.
  * A passive strategy describes a portfolio decision that avoids any direct or indirect security analysis.
  * A natural candidate for a passively held risky asset would be a well-diversified portfolio of common stocks.

| Period | U.S. Equity Market | 1-Month T-Bills | Excess Return | Standard Deviation | Sharpe Ratio |
|---|---|---|---|---|---|
| 1927-2018 | 11.72 | 3.38 | 8.34 | 20.36 | 0.41 |
| 1927-1949 | 9.40 | 0.92 | 8.49 | 26.83 | 0.32 |
| 1950-1972 | 14.00 | 3.14 | 10.86 | 17.46 | 0.62 |
| 1973-1995 | 13.38 | 7.26 | 6.11 | 18.43 | 0.33 |
| 1996-2018 | 10.10 | 2.21 | 7.89 | 18.39 | 0.43 |

## Markowitz Portfolio Optimization Model

**Portfolio Statistics**
| | Monthly | Annualized | | AMD | AMZN | FORD | JPM | NVDA | PFE | TGT | XOM |
|---|---|---|---|---|---|---|---|---|---|---|---|
| Port Mean | 1.88% | 25.05% | Mean | 0.95% | 1.69% | 0.15% | 0.87% | 2.34% | 0.26% | 0.73% | 0.64% |
| Port Variance | 0.0087 | 0.1044 | StdDev | 16.80% | 10.45% | 13.17% | 7.79% | 13.82% | 5.98% | 7.81% | 6.57% |
| Port Std Dev | 9.33% | 32.30% | | | | | | | | | |
| RF | 0.41% | 5.00% | | | | | | | | | |
| Sharpe Ratio | 0.1580 | | Weights | 0.00% | 43.44% | 0.00% | 12.05% | 44.51% | 0.00% | 0.00% | 0.00% |

**Constraints**
| | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 |
|---|---|---|---|---|---|---|---|---|---|

**Portfolio Variance**
| | AMD | AMZN | FORD | JPM | NVDA | PFE | TGT | XOM |
|---|---|---|---|---|---|---|---|---|
| 0.00% AMD | 0.000000 | 0.000000 | 0.000000 | 0.000000 | 0.000000 | 0.000000 | 0.000000 | 0.000000 |
| 43.44% AMZN | 0.000000 | 0.002060 | 0.000000 | 0.000086 | 0.001144 | 0.000000 | 0.000000 | 0.000000 |
| 0.00% FORD | 0.000000 | 0.000000 | 0.000000 | 0.000000 | 0.000000 | 0.000000 | 0.000000 | 0.000000 |
| 12.05% JPM | 0.000000 | 0.000086 | 0.000000 | 0.000088 | 0.000153 | 0.000000 | 0.000000 | 0.000000 |
| 44.51% NVDA | 0.000000 | 0.001144 | 0.000000 | 0.000153 | 0.003782 | 0.000000 | 0.000000 | 0.000000 |
| 0.00% PFE | 0.000000 | 0.000000 | 0.000000 | 0.000000 | 0.000000 | 0.000000 | 0.000000 | 0.000000 |
| 0.00% TGT | 0.000000 | 0.000000 | 0.000000 | 0.000000 | 0.000000 | 0.000000 | 0.000000 | 0.000000 |
| 0.00% XOM | 0.000000 | 0.000000 | 0.000000 | 0.000000 | 0.000000 | 0.000000 | 0.000000 | 0.000000 |
| Total | 0.008697 | 0.000000 | 0.003290 | 0.000000 | 0.000327 | 0.005079 | 0.000000 | 0.000000 | 0.000000 |

**Covariance Matrix**
| | AMD | AMZN | FORD | JPM | NVDA | PFE | TGT | XOM |
|---|---|---|---|---|---|---|---|---|
| AMD | 0.028238 | 0.007100 | 0.007415 | 0.004878 | 0.013188 | 0.002931 | 0.003786 | 0.001575 |
| AMZN | 0.007100 | 0.010915 | 0.003685 | 0.001647 | 0.005915 | 0.000905 | 0.001703 | 0.000677 |
| FORD | 0.007415 | 0.003685 | 0.017352 | 0.004850 | 0.005592 | 0.001378 | 0.003809 | 0.002817 |
| JPM | 0.004878 | 0.001647 | 0.004850 | 0.006061 | 0.002857 | 0.001776 | 0.002069 | 0.001799 |
| NVDA | 0.013188 | 0.005915 | 0.005592 | 0.002857 | 0.019092 | 0.001275 | 0.002959 | 0.001986 |
| PFE | 0.002931 | 0.000905 | 0.001378 | 0.001776 | 0.001275 | 0.003571 | 0.000867 | 0.000917 |
| TGT | 0.003786 | 0.001703 | 0.003809 | 0.002069 | 0.002959 | 0.000867 | 0.006099 | 0.000808 |
| XOM | 0.001575 | 0.000677 | 0.002817 | 0.001799 | 0.001986 | 0.000917 | 0.000808 | 0.004322 |

## What is next?
* Index Models and The Capital Asset Pricing Model
  * The Single-Index Model
  * The Capital Asset Pricing Model
  * Reading(s): BKM Ch. 8 & 9
  * Assignment #1 (Due before Lecture 11)
  * Suggested Problems
    * Ch. 7: 4-10, 12, 22-27.
    * Ch. 7 – CFA Problems: 1-4, 12.
```