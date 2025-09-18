```markdown
# Investments Finance 2 - BFIN

## Outline

*   Index Models and The Capital Asset Pricing Model
    *   The Single-Index Model
    *   The Capital Asset Pricing Model

## A Single-Factor Market

*   Advantages
    *   Reduces the number of inputs for diversification
        *   Suppose your security analysts can thoroughly analyze 50 stocks. This means that your input list will include the following:
            n = 50 estimates of expected returns
            n = 50 estimates of variances
            $(n^2 – n)/2$ = 1,225 estimates of covariances
            1,325 total estimates
    *   Easier for security analysts to specialize
*   Model
    $r_i = E(r_i) + \text{unanticipated surprise}$
    $r_i = E(r_i) + \beta_i m + e_i$

## A Single-Factor Market

*   Regression equation:
    $$R_i(t) = \alpha_i + \beta_i R_M(t) + e_i(t)$$
*   Expected return-beta relationship:
    $$E(R_i) = \alpha_i + \beta_i E(R_M)$$
*   Variance = Systematic risk + Firm-specific risk:
    $$\sigma_i^2 = \beta_i^2 \sigma_M^2 + \sigma^2(e_i)$$
*   Covariance = Product of betas $\times$ Market risk:
    $$\text{Cov}(r_i, r_j) = \beta_i \beta_j \sigma_M^2$$
*   Correlation =
    $$\text{Corr}(r_i, r_j) = \frac{\beta_i \beta_j \sigma_M^2}{\sigma_i \sigma_j} = \frac{\beta_i \sigma_M \beta_j \sigma_M}{\sigma_i \sigma_M \sigma_j \sigma_M}$$
    $$= \text{Corr}(r_i, r_m) \times \text{Corr}(r_j, r_m)$$

## A Single-Factor Market

*   Some securities will be more sensitive than others to macroeconomic shocks.
*   The variance of returns attributable to the marketwide factor is called the systematic risk of the security.
*   The index model assumes that firm-specific surprises are mutually uncorrelated:
    *   The only source of covariance between any pair of securities is their common dependence on the market return.
    $\text{Cov}(r_i, r_j) = \beta_i \beta_j \sigma_M^2$
    $\text{Corr}(r_i, r_j) = \text{Corr}(r_i, r_m) \times \text{Corr}(r_j, r_m)$

## A Single-Factor Market

$$R_i(t) = \alpha_i + \beta_i R_M(t) + e_i(t)$$
$$E(R_i) = \alpha_i + \beta_i E(R_M)$$

*   $\alpha$ is the security's expected excess return when the market excess return is zero. It is the vertical intercept.
*   The slope of the line in the figure is the security's beta coefficient, $\beta_i$.

## Opportunity Set of Risky Assets

The data below describe a three-stock financial market that satisfies the single-index model.

| Stock | Capitalization | Beta | Mean Excess Return | Standard Deviation |
| :---- | :------------- | :--- | :----------------- | :----------------- |
| A     | $3,000          | 1.0  | 10%                | 40%                |
| B     | 1,940          | 0.2  | 2                  | 30                 |
| C     | 1,360          | 1.7  | 17                 | 50                 |

The standard deviation of the market-index portfolio is 25%.
a. What is the mean excess return of the index portfolio?
b. What is the covariance between stock A and stock B?
c. What is the covariance between stock B and the index?
d. Break down the variance of stock B into its systematic and firm-specific components.

$\text{Cov}(r_i, r_j) = \beta_i \beta_j \sigma_M^2$
$\sigma_i^2 = \beta_i^2 \sigma_M^2 + \sigma^2(e_i)$

## Index Model Regression Equation

$$R_i(t) = \alpha_i + \beta_i R_{S\&P500}(t) + e_i(t)$$

| | Symbol |
| :------------------------------------------------------------------------------------------------------------------------------------------ | :------------------ |
| 1. The stock's expected return if the market is neutral, that is, if the market's excess return, $r_M - r_f$, is zero                            | $\alpha_i$          |
| 2. The component of return due to movements in the overall market in any period; $\beta_i$ is the security's responsiveness to market movements | $\beta_i(r_M - r_f)$ |
| 3. The unexpected component of return in any period due to unexpected events that are relevant only to this security (firm specific)            | $e_i$               |
| 4. The variance attributable to the uncertainty of the common macro-economic factor                                                         | $\beta_i^2 \sigma_M^2$ |
| 5. The variance attributable to firm-specific uncertainty                                                                                   | $\sigma^2(e_i)$     |

## Index Model Regression Equation

$$R_i(t) = \alpha_i + \beta_i R_{S\&P500}(t) + e_i(t)$$

### Regression statistics for Amazon

| Regression Statistics |        |
| :-------------------- | :----- |
| Multiple R            | 0.5351 |
| R-Square              | 0.2863 |
| Adjusted R-Square     | 0.2742 |
| Standard Error        | 0.0686 |
| Observations          | 60     |

|             | Coefficients | Standard Error | t-statistic | p-value |
| :---------- | :----------- | :------------- | :---------- | :------ |
| Intercept   | 0.0192       | 0.0093         | 2.0645      | 0.0434  |
| Market index| 1.5326       | 0.3150         | 4.8648      | 0.0000  |

*   The adjusted R-square corrects for an upward bias in R-square that arises because we use the estimated values of two parameters, the slope (beta) and intercept (alpha), rather than their true, but unobservable, values.
*   The standard error of the regression is the standard deviation of the residual, e.
    *   Higher the standard errors greater the impact of firm-specific events.

## Index Model Regression Equation

| Ticker | Company           | Beta   | Alpha  | R-Square | Residual Std Dev | Standard Error Beta | Standard Error Alpha | Adjusted Beta |
| :----- | :---------------- | :----- | :----- | :------- | :--------------- | :------------------ | :------------------- | :------------ |
| CPB    | Campbell Soup     | 0.247  | 0.001  | 0.012    | 0.064            | 0.292               | 0.009                | 0.498         |
| NEM    | Newmont Mining    | 0.430  | 0.005  | 0.011    | 0.117            | 0.538               | 0.016                | 0.620         |
| MCD    | McDonald's        | 0.563  | 0.006  | 0.165    | 0.036            | 0.165               | 0.005                | 0.709         |
| SBUX   | Starbucks         | 0.581  | 0.004  | 0.112    | 0.046            | 0.212               | 0.006                | 0.721         |
| KO     | Coca-Cola         | 0.663  | -0.001 | 0.258    | 0.032            | 0.146               | 0.004                | 0.776         |
| UNP    | Union Pacific     | 0.859  | 0.005  | 0.212    | 0.047            | 0.216               | 0.006                | 0.906         |
| PFE    | Pfizer            | 0.895  | -0.000 | 0.367    | 0.033            | 0.153               | 0.005                | 0.930         |
| XOM    | ExxonMobil        | 0.920  | -0.006 | 0.342    | 0.036            | 0.166               | 0.005                | 0.946         |
| MSFT   | Microsoft         | 0.923  | 0.012  | 0.193    | 0.054            | 0.246               | 0.007                | 0.948         |
| INTC   | Intel             | 0.934  | 0.007  | 0.187    | 0.055            | 0.254               | 0.007                | 0.956         |
| GOOG   | Alphabet (Google) | 0.960  | 0.008  | 0.209    | 0.053            | 0.243               | 0.007                | 0.973         |
| DIS    | Walt Disney       | 1.288  | -0.001 | 0.496    | 0.037            | 0.169               | 0.005                | 1.192         |
| BAC    | Bank of America   | 1.357  | 0.003  | 0.270    | 0.063            | 0.291               | 0.009                | 1.238         |
| BA     | Boeing            | 1.368  | 0.011  | 0.330    | 0.055            | 0.254               | 0.007                | 1.246         |
| AMZN   | Amazon            | 1.533  | 0.019  | 0.286    | 0.069            | 0.315               | 0.009                | 1.355         |
| MRO    | Marathon Oil      | 2.632  | -0.023 | 0.314    | 0.110            | 0.506               | 0.015                | 2.088         |
|        |                   |        |        |          |                  |                     |                      |               |
| AVERAGE|                   | 1.010  | 0.003  | 0.235    | 0.057            | 0.260               | 0.008                | 1.006         |
| STD DEVIATION |          | 0.560  | 0.009  | 0.127    | 0.025            | 0.115               | 0.003                | 0.374         |

## Index Model Regression Equation

### A. Weights in Optimal Risky Portfolio

|                   | Index Model | Full-Covariance Model |
| :---------------- | :---------- | :-------------------- |
| Market index      | 0.82        | 0.90                  |
| WMT (Walmart)     | 0.13        | 0.17                  |
| TGT (Target)      | -0.07       | -0.14                 |
| VZ (Verizon)      | -0.05       | -0.18                 |
| T (AT&T)          | 0.10        | 0.19                  |
| F (Amazon)        | 0.07        | 0.08                  |
| GM (General Motors)| 0.01        | -0.03                 |

### B. Portfolio Characteristics

|                   | Index Model | Full-Covariance Model |
| :---------------- | :---------- | :-------------------- |
| Risk premium      | 0.0605      | 0.0639                |
| Standard deviation| 0.1172      | 0.1238                |
| Sharpe ratio      | 0.5165      | 0.5163                |

*   Is the index model inferior to the full-blown Markowitz model?
    *   It imposes additional assumptions that may not be fully accurate.
    *   The Markowitz model allows far more flexibility in modeling asset covariance structure.
    *   Estimating the covariances with a sufficient degree of accuracy is an issue.

## The Capital Asset Pricing Model

*   Portfolio Theory vs. CAPM
    *   Mean-Variance Analysis
        *   Tells us how to select a portfolio given expected returns, variances, and covariances.
        *   Does not tell us anything about what prices should be.
    *   CAPM
        *   An equilibrium model that characterizes risk-return combinations of securities that occur when investors are mean-variance optimizers.
        *   The term equilibrium refers to a situation where no investor wants to do anything differently.
        *   It is the equilibrium model that underlies all modern financial theory.

## The Capital Asset Pricing Model

*   The CAPM can be derived by asking the question:
    *   If everybody in the economy holds an efficient portfolio, what do prices need to be so that markets clear?
    *   Suppose that based on the prices/expected returns our model comes up with, we find that IBM does not enter into any maximizing investor's portfolio.
        *   Then IBM must be priced too high
        *   Since nobody will hold IBM shares at that price, the price will fall to a point where the aggregate demand of investors equals the number of IBM shares outstanding.

## The Capital Asset Pricing Model

*   Modern Portfolio Theory tells us that every investor holds a combination of just two portfolios
    *   The risk-free asset
    *   The tangency portfolio
*   Thus, the tangency portfolio must be the market portfolio
    *   The market portfolio consists of all risky assets held in proportion to their market value
    *   Stocks, bonds, real estate, human capital, etc.

## The Capital Asset Pricing Model

*   The CAPM Assumptions
    *   All investors are rational mean-variance optimizers with identical planning horizons.
    *   Investors can borrow or lend any amount at a fixed, risk-free rate.
    *   Perfect competition: no individual investor can affect security prices.
    *   All assets are tradable and perfectly divisible.
    *   No taxes, transaction costs, or short-sale constraints.
    *   Investors have homogeneous expectations.
        *   They agree on the estimates of expected returns, variances, and covariances.

## The Capital Asset Pricing Model

*   The CAPM –Main Result
    $$E[R_i] = r_f + \beta_i \times (E[R_{Mkt}] - r_f)$$
    Risk premium for security i
    Volatility of i that is common with the market
    $$\beta_i = \frac{\text{SD}(R_i) \times \text{Corr}(R_i, R_{Mkt})}{\text{SD}(R_{Mkt})} = \frac{\text{Cov}(R_i, R_{Mkt})}{\text{Var}(R_{Mkt})}$$
*   Security Market Line (SML)
    *   Plots the expected return of assets against their beta.
    *   The CAPM states that all assets must be on the SML.
*   SML vs CML
    *   SML
        *   Shows systematic risk only
        *   Every security / portfolio lies on the SML
    *   CML
        *   Shows the total risk (systematic + unsystematic)
        *   Only two securities lie on the CML
            *   Risk-free asset and the market portfolio

## The Capital Asset Pricing Model

### A: The Efficient Frontier of Risky Assets with the Optimal CAL
### B: The Efficient Frontier and the Capital Market Line

## The Capital Asset Pricing Model

## The Capital Asset Pricing Model

*   The risk premium on the market portfolio is proportional to its risk and the degree of risk aversion:
    $$E(R_M) = \bar{A} \sigma_M^2$$
    *   An individual security's risk premium is a function of:
        *   Its contribution to the risk of the market portfolio
        *   The covariance of returns with the assets that make up the market portfolio
    $$\sum_{i=1}^{n} w_i \text{Cov}(R_i, R_{GE}) = \text{Cov}\left(\sum_{i=1}^{n} w_i R_i, R_{GE}\right)$$
    $$\frac{\text{GE's contribution to risk premium}}{\text{GE's contribution to variance}} = \frac{w_{GE} E(R_{GE})}{w_{GE} \text{Cov}(R_{GE}, R_M)} = \frac{E(R_{GE})}{\text{Cov}(R_{GE}, R_M)}$$
    $$\frac{\text{Market risk premium}}{\text{Market variance}} = \frac{E(R_M)}{\sigma^2(R_M)}$$
    $$E(R_{GE}) = \frac{\text{Cov}(R_{GE}, R_M)}{\sigma^2(R_M)} E(R_M)$$
    $$E(r_{GE}) = r_f + \beta_{GE}[E(r_M) - r_f]$$
    Expected return-beta relationship

## The Capital Asset Pricing Model

*   CAPM holds for the overall portfolio because:
    $$E(r_P) = \sum_k w_k E(r_k)$$
    $$\beta_P = \sum_k w_k \beta_k$$
*   This also holds for the market portfolio:
    $$E(r_M) = r_f + \beta_M [E(r_M) - r_f]$$

## The Capital Asset Pricing Model

*   An asset that is not priced according to the CAPM will not line up on the SML.
*   The difference between its actual risk premium and its risk premium predicted by the CAPM is called the asset's alpha:
    $$E(r_i) - r_f = \alpha_i + \beta_i[E(r_M) - r_f]$$

## The Capital Asset Pricing Model

*   The Equity Cost of Capital
    *   Best expected return available in the market on investments with similar risk.
    *   Under the CAPM?
        *   Investments have similar risk if they have the same sensitivity to market risk, as measured by their beta with the market portfolio.
*   The Market Portfolio
    *   Value-weighted vs. equal-weighted
    *   S&P 500, DJIA, NDQ, S&P 1500 Composite, Russel 2000, Wilshire 5000.
*   The Market Risk Premium
    *   Risk-Free Rate
        *   Maturity vs. investment horizon
    *   The Risk Premium
        *   Historical
        *   Expected

| Period                    |               |
| :------------------------ | :------------ |
| S&P 500 Excess Return Versus | 1926–2015 | 1965–2015 |
| One-year Treasury         | 7.7%          | 5.0%      |
| Ten-year Treasury*        | 5.9%          | 3.9%      |

## The Capital Asset Pricing Model

*   Beta Estimation
    *   Using Historical Returns
        *   What is the assumption?
    *   Best-fitting line
        *   Beta corresponds to the slope of the best-fitting line in the plot of the security's excess returns vs. the market excess return.
    *   Linear Regression
    $$ (R_i - r_f) = \alpha_i + \beta_i(R_M - r_f) + e_i $$

## The Capital Asset Pricing Model

## The Capital Asset Pricing Model

*   Historical Betas
    $$r_{i,t}^e = \alpha_i + \beta_i r_{M,t}^e + \epsilon_{i,t}$$
    $$\text{S.E.}(\hat{\beta}_i) = \frac{\sqrt{1-R^2}}{\sqrt{T}} \frac{\hat{\sigma}_i}{\hat{\sigma}_M}$$
*   The precision of an OLS beta estimate can be increased by
    *   Increasing the number of observations (T),
    *   By using portfolios instead of individual securities,
    *   By increasing the frequency of return observations

## The Capital Asset Pricing Model

*   Should idiosyncratic risk matter for pricing?
*   Would you ever buy a stock with negative expected returns?
*   How do the betas add up?
*   Can you arbitrage stocks that are on the SML?
*   Can you arbitrage stocks that are not on the SML?

## What is next?

*   Multifactor Models
*   Arbitrage Pricing Theory
*   Reading(s): BKM Ch. 10
*   Suggested Problems
    *   Ch.8: 6, 9-12
    *   Ch.9: 2, 4, 8, 17-19, 21.
    *   Ch.9-CFA Problems: 1-2, 8-9,12.
```