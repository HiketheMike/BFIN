```markdown
# Investments Finance 2 - BFIN

## Outline
*   Portfolio Theory and Practice I
    *   Risk, Return, and the Historical Record
    *   Capital Allocation to Risky Assets

## Return on Investments
*   Total Return (Holding Period Return)
    *   The total return realized on an investment in a given period and has two components:
        *   Capital gains in the relevant period,
        *   Income generated during the period (Dividend, coupon, rent, etc.)

$$TR = \frac{P_1 - P_0 + I}{P_0}$$

| TR  | Total return                               |
| :-- | :----------------------------------------- |
| P1  | The price of the asset at the end of the period    |
| P0  | The price of the asset at the beginning of the period |
| I   | Income generated during the holding period |

*   Total return calculations do not take the return on reinvestment of the income earned during the period into account.
*   The holding period return is not a standardized value in terms of time.

## Return on Investments
Expected Ending Price = \$110
Beginning Price = \$100
Expected Dividend = \$4

$$HPR = \frac{E(P_1) - P_0 + E(D_1)}{P_0} = \frac{\$110 - \$100 + \$4}{\$100}$$
$$= \frac{\$110 - \$100}{\$100} + \frac{\$4}{\$100}$$
$$= 10\% + 4\% = 14\% \longleftarrow \text{Holding Period Return}$$
Capital Gains Yield $\uparrow$ Dividend Yield $\uparrow$

## Return on Investments
$$TR_{Annual} = [1 + TR]^{1/N} - 1$$

An investor bought stocks of AGE, Inc. at a price of €25 On January 01, 2022. The company paid a dividend of €1 per share on 30 June 2022. The investor sold the stock at a price of €30 on January 31, 2023. Calculate the holding period return and the annualized total return.

$$TR = \frac{P_1 - P_0 + D}{P_0}$$
$$TR = \frac{30 - 25 + 1}{25}$$
$$TR = \frac{6}{25} = \%24$$
$$TR_{Annual} = [1 + TR]^{1/N} - 1$$
$$TR_{Annual} = [1 + 0,24]^{13/12} - 1 = \%21,97$$

## Return on Investments
On January 01, 2021, an investor purchased government bond with a face value of €1,000 and a maturity of 5 years at a price of €1,100. The bond makes coupon payments of €60 on 30 June and 31 December. The investor sold the bonds on 30 June 2022 at a price of €1,058. What is the investor's holding period return and the annual total return?

$$TR = \frac{P_1 - P_0 + C}{P_0}$$
$$TR = \frac{1058 - 1100 + (60*3)}{1100}$$
$$TR = \frac{138}{1100} = \%12,55$$
$$TR_{Annual} = [1 + TR]^{1/N} - 1$$
$$TR_{Annual} = [1 + 0,1255]^{3/2} - 1$$
$$TR_{Annual} = [1 + 0,1255]^2 - 1$$
$$TR_{Annual} = 8,20\%$$

## Return on Investments
Image: S&P 500 Price and Total Return Indices chart.

## Return on Investments
*   Expected Return
    *   When investors purchase an asset, the level of total return they will realize during their holding period involves uncertainty.
    *   The expected rate of return is the probability-weighted average of the rates of return that will occur in each scenario.

$$E(r) = \sum_s p(s) \times r(s)$$

| $P_0$ (€) | 20 |
| :-------- | :- |

| Market Conditions | Probability | Stock Price | Dividend | Total Return | TR*Prob. |
| :---------------- | :---------- | :---------- | :------- | :----------- | :------- |
| Perfect           | 10%         | 29          | 1.50     | 0.5250       | 0.053    |
| Good              | 25%         | 26          | 1.25     | 0.3625       | 0.091    |
| Flat              | 35%         | 23          | 1.00     | 0.2000       | 0.070    |
| Bad               | 25%         | 16          | 0.25     | -0.1875      | -0.047   |
| Crisis            | 5%          | 10          | 0.00     | -0.5000      | -0.025   |
|                   | 100%        |             |          | **Expected Return** | **14.13%** |

Where,
$p(s)$ = Probability of a state
$r(s)$ = Return if a state occurs
$s$ = State

## Return on Investments
*   Excess Return
    *   The return differential between a risky asset and a risk-free asset in any given period.
    *   Also called the risk premium.
    *   The risk-free rate is the rate of interest on an instrument that has no default risk and reinvestment risk.
    *   The risk-free interest rate in real and nominal terms:
    $$r_{f,real} = \frac{1 + r_{f,nominal}}{1 + e} - 1$$

| $P_0$ | 20   |
| :---- | :--- |
| $r_f$ | 0.08 |

| Market Conditions | Probability | Stock Price | Dividend | Total Return | Excess Return | (TR-$r_f$)*Prob. |
| :---------------- | :---------- | :---------- | :------- | :----------- | :------------ | :---------------- |
| Perfect           | 10%         | 29          | 1.50     | 0.5250       | 0.4450        | 0.045             |
| Good              | 25%         | 26          | 1.25     | 0.3625       | 0.2825        | 0.071             |
| Flat              | 35%         | 23          | 1.00     | 0.2000       | 0.1200        | 0.042             |
| Bad               | 25%         | 16          | 0.25     | -0.1875      | -0.2675       | -0.067            |
| Crisis            | 5%          | 10          | 0.00     | -0.5000      | -0.5800       | -0.029            |
|                   | 100%        |             |          |              | **Expected Excess Return** | **6.13%**         |

## Risk in Investments
*   Two of the fundamental questions of investments:
    *   What is risk and how can we measure it?
    *   How much additional return should we earn for bearing an additional unit of risk?

## Risk in Investments
*   One of the main functions of financial markets is to enable economic agents to transfer their risks to willing counterparties or to assume the risks of others.
*   Financial risks are generally associated with uncertainty about the outcome of an investment.
*   Accordingly, volatility (variance) in returns is the main risk criterion.
*   Risk measures are not limited to volatility:
    *   VaR (Value at Risk)
        *   Measures the potential loss in value of a risky asset or portfolio over a defined period for a given confidence interval.
    *   Expected Shortfall or CVaR (Conditional Value at Risk)
        *   The expected loss given that the loss is greater than or equal to the VaR.
        *   Quantifies the losses that might be encountered in the tail.
    *   Semivariance
        *   Measures the dispersion of all observations that fall below the mean or target value of a set of data.
    *   Sortino Ratio
        *   The ratio of average excess returns to semivariance

## Risk in Investments
*   Modern portfolio theory and asset pricing models often begin with the assumption of a normal distribution of returns.
*   The normality assumption ensures that the standard deviation is an exact measure of risk.

Image: Normal distribution curve showing 68.26%, 95.44%, 99.74% within 1, 2, and 3 standard deviations from the mean.

*   A normal distribution;
    *   Fully defined by its mean ($\mu$) and variance ($\sigma^2$).
    *   Symmetrical, bell-shaped curve.
*   The mean of the standard normal distribution is 0 and the variance is 1.

## Risk in Investments
Image: Two plots of normal distributions with different means and variances.

*   The mean or expected value ($\mu$) of the distribution is known as the location parameter.
*   A normal distribution with $\mu \ne 0$ can be easily converted to a standard normal distribution ($\mu = 0$, $\sigma = 1$).
*   The standard deviation ($\sigma$) of the distribution is known as the distribution parameter.
*   When $\mu$ is constant, changes in distribution parameter affect the shape of the distribution.
*   Kurtosis is a measure of the "tailedness" of the probability distribution. A standard normal distribution has kurtosis of 3.

## Risk in Investments
Image: Histograms of various stock/index returns (SP500, NDQ100, EEM, XAU, AMD, AMZN, FORD, JPM, NVDA, PFE, TGT, XOM).

## Risk in Investments

|       | SP500    | NDQ100   | EEM      | FORD     | AMZN     | NVDA     | TGT      | AMD      | XOM      | PFE      | JPM      | XAU      |
| :---- | :------- | :------- | :------- | :------- | :------- | :------- | :------- | :------- | :------- | :------- | :------- | :------- |
| Mean  | 0.77%    | 1.09%    | 0.49%    | 0.15%    | 1.69%    | 2.34%    | 0.73%    | 0.95%    | 0.64%    | 0.26%    | 0.87%    | 0.67%    |
| Standard Error | 0.28%    | 0.34%    | 0.40%    | 0.85%    | 0.67%    | 0.89%    | 0.50%    | 1.08%    | 0.42%    | 0.39%    | 0.50%    | 0.31%    |
| Median| 1.38%    | 1.79%    | 0.77%    | -0.18%   | 2.25%    | 3.18%    | 0.42%    | 0.35%    | 0.70%    | 0.33%    | 1.24%    | 0.35%    |
| Standard Deviation | 4.33%    | 5.30%    | 6.24%    | 13.17%   | 10.45%   | 13.82%   | 7.81%    | 16.80%   | 6.57%    | 5.98%    | 7.79%    | 4.82%    |
| Sample Variance | 0.0019   | 0.0028   | 0.0039   | 0.0174   | 0.0109   | 0.0191   | 0.0061   | 0.0282   | 0.0043   | 0.0036   | 0.0061   | 0.0023   |
| CoV   | 0.3624   | 0.3142   | 0.8300   | 5.7714   | 0.3990   | 0.3811   | 0.6953   | 1.1359   | 0.6589   | 1.4931   | 0.5792   | 0.4661   |
| Kurtosis| 1.80     | 0.67     | 2.18     | 13.25    | 1.92     | 0.98     | 1.59     | 0.16     | 2.68     | 0.68     | 1.47     | 0.60     |
| Skewness| -0.78    | -0.57    | -0.52    | -0.15    | -0.21    | -0.42    | -0.26    | -0.18    | -0.12    | -0.03    | -0.55    | -0.16    |
| Range | 0.30     | 0.32     | 0.45     | 1.68     | 0.80     | 0.96     | 0.56     | 0.95     | 0.53     | 0.40     | 0.47     | 0.31     |
| Minimum| -18.39%  | -17.77%  | -29.52%  | -86.11%  | -36.49%  | -50.31%  | -34.54%  | -52.85%  | -28.92%  | -19.46%  | -25.70%  | -18.45%  |
| Maximum| 12.06%   | 14.18%   | 15.54%   | 82.37%   | 43.35%   | 45.20%   | 21.42%   | 42.13%   | 23.83%   | 20.57%   | 21.64%   | 12.06%   |
| Count | 240      | 240      | 240      | 240      | 240      | 240      | 240      | 240      | 240      | 240      | 240      | 240      |

*   A distribution with no skew, such as a normal distribution, is symmetrical, with the mean, median, and mode all being equal.
*   A positively skewed distribution is a type of data distribution where most of the data points are clustered towards the lower end of the spectrum, with a smaller number of outliers near the higher end.
*   A negatively skewed distribution is a distribution where the majority of values are concentrated on the right side of the distribution graph, while the left tail is longer.
*   Coefficient of variation (CoV): Quantifies the relative variability in relation to the mean.

## Risk in Investments
Variance (VAR):
$$\sigma^2 = \sum_s p(s) \times [r(s) - E(r)]^2$$
Standard Deviation (STD):
$$STD = \sqrt{\sigma^2}$$

| State     | Prob. of State | r in State |
| :-------- | :------------- | :--------- |
| Excellent | .25            | 0.3100     |
| Good      | .45            | 0.1400     |
| Poor      | .25            | -0.0675    |
| Crash     | .05            | -0.5200    |

$E(r) = (.25) \times (.31) + (.45) \times (.14) + (.25) \times (-.0675) + (0.05) \times (-0.52)$
$E(r) = 9.76\%$
$\sigma^2 = .25 \times (.31 – 0.0976)^2 + .45 \times (.14 – .0976)^2 + .25 \times (-0.0675 – 0.0976)^2 + .05 \times (-.52 – .0976)^2 = .038$
$\sigma = \sqrt{.038} = .1949$

## Risk in Investments
$$E(r_i) = p_1r_1 + p_2r_2 + \cdots + p_nr_n$$
$$\sigma^2(r_i) = p_1 \times (r_1 - E(r_i))^2 + p_2 \times (r_2 - E(r_i))^2 + \cdots + p_n \times (r_n - E(r_i))^2$$
$$\sigma = \sqrt{\sigma^2(r_i)}$$

| Scenario | Prob. | Return  | Deviations           |
| :------- | :---- | :------ | :------------------- |
|          | $p_n$ | $r_n$   | $p_n \times [r_n-E(r_i)]^2$ |
| 1        | 15%   | 9.0%    | 0.000005             |
| 2        | 20%   | 8.0%    | 0.000048             |
| 3        | 10%   | 6.0%    | 0.000126             |
| 4        | 30%   | 10.0%   | 0.000006             |
| 5        | 25%   | 12.0%   | 0.000150             |
|          | 100%  | **9.55%** | **0.000335**         |
|          |       | $E(r_i)$ | $\sigma^2$           |

## Risk in Investments

| $P_0$ | 20   |
| :---- | :--- |
| $r_f$ | 0.08 |

| Market Conditions | Prob. | Stock Price | Dividend | Total Return | TR*Prob. | TR Deviations | Excess Return | (TR-$r_f$)*Prob. | Excess Return Deviations |
| :---------------- | :---- | :---------- | :------- | :----------- | :------- | :------------ | :------------ | :---------------- | :----------------------- |
| Perfect           | 10%   | 29          | 1.50     | 0.5250       | 0.0525   | 0.0147        | 0.4450        | 0.045             | 0.0147                   |
| Good              | 25%   | 26          | 1.25     | 0.3625       | 0.0906   | 0.0122        | 0.2825        | 0.071             | 0.0122                   |
| Flat              | 35%   | 23          | 1.00     | 0.2000       | 0.0700   | 0.0012        | 0.1200        | 0.042             | 0.0012                   |
| Bad               | 25%   | 16          | 0.25     | -0.1875      | -0.0469  | 0.0270        | -0.2675       | -0.067            | 0.0270                   |
| Crisis            | 5%    | 10          | 0.00     | -0.5000      | -0.0250  | 0.0206        | -0.5800       | -0.029            | 0.0206                   |
|                   | 100%  |             |          |              | 14.13%   | **0.0758**    |               | 6.13%             | **0.0758**               |
|                   |       |             |          |              | $E(r_i)$ | $\sigma^2$    |               | $E(r_i) - r_f$    | $\sigma^2$               |

## Risk in Investments
Image: Historical Average Return vs Historical Volatility (standard deviation) chart for various asset classes (Treasury Bills, Corporate Bonds, World Portfolio, S&P 500, Mid-Cap Stocks, Small Stocks) with an indicated historical excess return for S&P 500 over TBills.

## Risk in Investments
Image: "Risk & Return (Monthly, 2004-2013)" scatter plot for various stocks/indices.
Image: "Risk & Return (Monthly, 2014-2023)" scatter plot for various stocks/indices.

## Risk in Investments
Image: "Risk & Return (Monthly, 2004-2023)" scatter plot for various stocks/indices.

## Risk in Investments
*   True means and variances are unobservable
    *   Possible scenarios like the ones we used in the examples are unknown
*   Means and variances must be estimated
*   Arithmetic Average
    $$E(r) = \sum_{s=1}^n p(s)r(s) = \frac{1}{n} \sum_{s=1}^n r(s)$$
*   Geometric (Time-Weighted) Average
    *   Terminal value of the investment:
        $$TV_n = (1 + r_1)(1 + r_2)\dots(1 + r_n)$$
    *   Geometric Average:
        $$g = TV_n^{1/n} - 1$$

## Risk in Investments
*   Estimated Variance
    *   Expected value of squared deviations
        $$\hat{\sigma}^2 = \frac{1}{n} \sum_{s=1}^n [r(s) - \bar{r}]^2$$
    *   Unbiased estimated standard deviation
        $$\hat{\sigma} = \sqrt{\frac{1}{n-1} \sum_{j=1}^n [r(s) - \bar{r}]^2}$$
*   Sharpe Ratio
    $$\frac{\text{Risk premium}}{\text{SD of excess returns}}$$

## Risk in Investments
*   Symmetric Returns
    *   Standard deviation is a good measure of risk
    *   Portfolio returns will also be symmetric
    *   Only mean and standard deviation needed to estimate future scenarios
    *   Pairwise correlation coefficients summarize the dependence of returns across securities
*   What if excess returns are not normally distributed?
    *   STD is no longer a complete measure of risk
    *   Skewness:
        $$Skew = Average \left[\frac{(R - \bar{R})^3}{\hat{\sigma}^3}\right]$$
    *   Kurtosis:
        $$Kurtosis = Average \left[\frac{(R - \bar{R})^4}{\hat{\sigma}^4}\right] - 3$$
    *   Sharpe ratio is not a complete measure of portfolio performance

## Risk in Investments
*   Normal distribution is generally a good approximation of returns
    *   VaR indicates no greater tail risk than equivalent normal
    *   ES $\le 0.41$ of monthly SD $\implies$ no evidence against normality
*   However
    *   Negative skew is present in some portfolios some of the time
    *   Positive kurtosis is present in all portfolios all the time

## Risk and Risk Aversion
*   Speculation
    *   Taking a considerable risk for a commensurate gain
    *   Parties have heterogeneous expectations
*   Gambling
    *   Bet on an uncertain outcome for enjoyment
    *   Parties assign the same probabilities to the possible outcomes
*   Utility Values
    *   Investors are willing to consider:
        *   Risk-free assets
        *   Speculative positions with positive risk premiums
    *   Portfolio attractiveness
        *   Increases with expected return
        *   Decreases with risk
        *   What happens when return increases with risk?

## Risk and Risk Aversion
*   Utility Function
    $$U = E(r) - \frac{1}{2}A\sigma^2$$
    *   U = Utility
    *   E(r) = Expected return on the asset or portfolio
    *   A = Coefficient of risk aversion
    *   $\sigma^2$ = Variance of returns
    *   $1/2$ = A scaling factor
*   Risk Averse Investors:
    $$A > 0$$
*   Risk-Neutral Investors:
    $$A = 0$$
*   Risk Lovers:
    $$A < 0$$

## Risk and Risk Aversion
$$U = E(r) - \frac{1}{2}A\sigma^2$$

| Portfolio       | Risk Premium | Expected Return | Risk (SD) |
| :-------------- | :----------- | :-------------- | :-------- |
| L (low risk)    | 2%           | 7%              | 5%        |
| M (medium risk) | 4            | 9               | 10        |
| H (high risk)   | 8            | 13              | 20        |

| Investor Risk Aversion (A) | Utility Score of Portfolio L [E(r) = .07; $\sigma$ = .05] | Utility Score of Portfolio M [E(r) = .09; $\sigma$ = .10] | Utility Score of Portfolio H [E(r) = .13; $\sigma$ = .20] |
| :------------------------- | :------------------------------------------------------- | :------------------------------------------------------- | :------------------------------------------------------- |
| 2.0                        | $.07 - \frac{1}{2} \times 2 \times .05^2 = .0675$          | $.09 - \frac{1}{2} \times 2 \times .1^2 = .0800$          | $.13 - \frac{1}{2} \times 2 \times .2^2 = .09$           |
| 3.5                        | $.07 - \frac{1}{2} \times 3.5 \times .05^2 = .0656$        | $.09 - \frac{1}{2} \times 3.5 \times .1^2 = .0725$        | $.13 - \frac{1}{2} \times 3.5 \times .2^2 = .06$         |
| 5.0                        | $.07 - \frac{1}{2} \times 5 \times .05^2 = .0638$          | $.09 - \frac{1}{2} \times 5 \times .1^2 = .0650$          | $.13 - \frac{1}{2} \times 5 \times .2^2 = .03$           |

## Risk and Risk Aversion
*   Mean-Variance (M-V) Criterion
    *   Portfolio X dominates portfolio Y if:
        $E(r_X) \ge E(r_Y)$ and $\sigma_X \le \sigma_Y$ and at least one inequality is strict
*   Indifference Curves
    *   Equally preferred portfolios will lie in the mean-standard deviation plane on an indifference curve
    *   All portfolio points with the same utility value

Image: Indifference Curve chart showing expected return E(r) versus standard deviation $\sigma$.

## Portfolio Return
*   In a portfolio of multiple assets, the return of the portfolio over a given period is the weighted average of the returns of each asset.
    $$r_p = w_1r_1 + w_2r_2 + \cdots + w_Nr_N$$
    $$r_p = \sum_{n=1}^N w_nr_n$$

| Asset | Price  | Units  | Value (t=0) | Weight in Portfolio | TR     | Value (t=1) |
| :---- | :----- | :----- | :---------- | :------------------ | :----- | :---------- |
| A     | 120.00 | 5.00   | 600.00      | 20.0%               | 12.0%  | 672.00      |
| B     | 5.00   | 150.00 | 750.00      | 25.0%               | 30.0%  | 975.00      |
| C     | 90.00  | 10.00  | 900.00      | 30.0%               | 5.0%   | 945.00      |
| D     | 30.00  | 15.00  | 450.00      | 15.0%               | 10.0%  | 495.00      |
| E     | 12.00  | 25.00  | 300.00      | 10.0%               | -10.0% | 270.00      |
|       |        |        | **3,000.00**| **100.0%**          | **11.9%**| **3,357.00**|
|       |        |        | Portfolio Value (t=0) |                     | TR on the Portfolio | Portfolio Value (t=1) |

## Portfolio Return
*   In a portfolio with more than one asset, the expected return in a given period is the weighted average of the expected returns on the assets in the portfolio.
    $$E(r_p) = w_1E(r_1) + w_2E(r_2) + \cdots + w_NE(r_N)$$
    $$E(r_p) = \sum_{n=1}^N w_nE(r_n)$$

| Market Conditions | Prob. | Asset A (w=0.40) |                  | Asset B (w=0.60) |                  |
| :---------------- | :---- | :--------------- | :--------------- | :--------------- | :--------------- |
|                   |       | TR               | TR*Prob.         | TR               | TR*Prob.         |
| 1                 | 25%   | 12.0%            | 3.0%             | 6.0%             | 1.5%             |
| 2                 | 15%   | 11.0%            | 1.7%             | 8.0%             | 1.2%             |
| 3                 | 35%   | 10.0%            | 3.5%             | 10.0%            | 3.5%             |
| 4                 | 15%   | 9.0%             | 1.4%             | 12.0%            | 1.8%             |
| 5                 | 10%   | 6.0%             | 0.6%             | 14.0%            | 1.4%             |
|                   | **100%** |                  | **10.10%**       |                  | **9.40%**        |

$E(r_p) = w_AE(r_A) + w_BE(r_B)$
$E(r_p) = 0,40 \times 0,1010 + 0,60 \times 0,0940 = 9,68\%$

## Portfolio Risk
$$E(r_i) = p_1r_1 + p_2r_2 + \cdots + p_nr_n$$
$$\sigma^2(r_i) = p_1 \times (r_1 - E(r_i))^2 + p_2 \times (r_2 - E(r_i))^2 + \cdots + p_n \times (r_n - E(r_i))^2$$
$$\sigma = \sqrt{\sigma^2(r_i)}$$

| Market Conditions | Prob. | TR    | TR*Prob. | Asset A $(r_n-E(r_n))$ | $(r_n-E(r_n))^2$ | Prob.*$(r_n-E(r_n))^2$ | TR    | TR*Prob. | Asset B $(r_n-E(r_n))$ | $(r_n-E(r_n))^2$ | Prob.*$(r_n-E(r_n))^2$ |
| :---------------- | :---- | :---- | :------- | :---------------------- | :--------------- | :---------------------- | :---- | :------- | :---------------------- | :--------------- | :---------------------- |
| 1                 | 25%   | 12.0% | 3.0%     | 1.9%                    | 0.0004           | 0.00009                 | 6.0%  | 1.5%     | -3.4%                   | 0.0012           | 0.00029                 |
| 2                 | 15%   | 11.0% | 1.7%     | 0.9%                    | 0.0001           | 0.00001                 | 8.0%  | 1.2%     | -1.4%                   | 0.0002           | 0.00003                 |
| 3                 | 35%   | 10.0% | 3.5%     | -0.1%                   | 0.0000           | 0.00000                 | 10.0% | 3.5%     | 0.6%                    | 0.0000           | 0.00001                 |
| 4                 | 15%   | 9.0%  | 1.4%     | -1.1%                   | 0.0001           | 0.00002                 | 12.0% | 1.8%     | 2.6%                    | 0.0007           | 0.00010                 |
| 5                 | 10%   | 6.0%  | 0.6%     | -4.1%                   | 0.0017           | 0.00017                 | 14.0% | 1.4%     | 4.6%                    | 0.0021           | 0.00021                 |
|                   | 100%  |       | 10.10%   |                         |                  | $\sigma^2$ = **0.00029**|       | 9.40%    |                         |                  | $\sigma^2$ = **0.00064**|
|                   |       |       |          |                         |                  | $\sigma$ = **0.0170**   |       |          |                         |                  | $\sigma$ = **0.0254**   |

## Portfolio Risk

| Market Conditions | Prob. | TR    | TR*Prob. | Asset A $(r_n-E(r_n))$ | $(r_n-E(r_n))^2$ | Prob.*$(r_n-E(r_n))^2$ | TR    | TR*Prob. | Asset B $(r_n-E(r_n))$ | $(r_n-E(r_n))^2$ | Prob.*$(r_n-E(r_n))^2$ |
| :---------------- | :---- | :---- | :------- | :---------------------- | :--------------- | :---------------------- | :---- | :------- | :---------------------- | :--------------- | :---------------------- |
| 1                 | 25%   | 12.0% | 3.0%     | 1.9%                    | 0.0004           | 0.00009                 | 6.0%  | 1.5%     | -3.4%                   | 0.0012           | 0.00029                 |
| 2                 | 15%   | 11.0% | 1.7%     | 0.9%                    | 0.0001           | 0.00001                 | 8.0%  | 1.2%     | -1.4%                   | 0.0002           | 0.00003                 |
| 3                 | 35%   | 10.0% | 3.5%     | -0.1%                   | 0.0000           | 0.00000                 | 10.0% | 3.5%     | 0.6%                    | 0.0000           | 0.00001                 |
| 4                 | 15%   | 9.0%  | 1.4%     | -1.1%                   | 0.0001           | 0.00002                 | 12.0% | 1.8%     | 2.6%                    | 0.0007           | 0.00010                 |
| 5                 | 10%   | 6.0%  | 0.6%     | -4.1%                   | 0.0017           | 0.00017                 | 14.0% | 1.4%     | 4.6%                    | 0.0021           | 0.00021                 |
|                   | 100%  |       | 10.10%   |                         |                  | $\sigma^2$ = **0.00029**|       | 9.40%    |                         |                  | $\sigma^2$ = **0.00064**|
|                   |       |       |          |                         |                  | $\sigma$ = **0.0170**   |       |          |                         |                  | $\sigma$ = **0.0254**   |

*   For an asset, the variance is a measure of the dispersion of possible returns on the asset around the expected return.
*   Similarly, portfolio variance measures the dispersion of possible portfolio returns around the expected portfolio return.
*   How should we calculate the standard deviation (risk) of the portfolio consisting of these two assets?

## Portfolio Risk
*   When calculating the expected return of the portfolio, we take the weighted average of the expected returns of the assets.
*   We cannot use the same method for variance or standard deviation.
*   Covariance;
    *   The relationship between the changes in the returns of two assets.
    *   When viewed at the portfolio level, the sign and size of the covariance will have an impact on the final volatility of the portfolio.
*   For two assets;
    $$cov(r_i, r_j) = p_1 \times [r_{i1} - E(r_i)] \times [r_{j1} - E(r_j)] +$$
    $$p_2 \times [r_{i2} - E(r_i)] \times [r_{j2} - E(r_j)] + \cdots$$
    $$+ p_N \times [r_{iN} - E(r_i)] \times [r_{jN} - E(r_j)]$$

## Portfolio Risk
*   Covariance;
    *   The relationship between the changes in the returns of two assets.

| Market Conditions | Prob. | $TR_A$ | $(r_A-E(r_A))$ | $TR_B$ | $(r_B-E(r_B))$ | $p \times (r_A-E(r_A)) \times (r_B-E(r_B))$ |
| :---------------- | :---- | :----- | :------------- | :----- | :------------- | :------------------------------------------- |
| 1                 | 25%   | 12.0%  | 1.9%           | 6.0%   | -3.4%          | -0.000162                                    |
| 2                 | 15%   | 11.0%  | 0.9%           | 8.0%   | -1.4%          | -0.000019                                    |
| 3                 | 35%   | 10.0%  | -0.1%          | 10.0%  | 0.6%           | -0.000002                                    |
| 4                 | 15%   | 9.0%   | -1.1%          | 12.0%  | 2.6%           | -0.000043                                    |
| 5                 | 10%   | 6.0%   | -4.1%          | 14.0%  | 4.6%           | -0.000189                                    |
|                   | 100%  | 10.10% |                | 9.40%  |                | Cov($r_A$, $r_B$) = **-0.000414**           |

## Portfolio Risk
*   A concept closely related to covariance is the correlation.
    *   Covariance is not a standardized measure.
    *   Correlation is a function of covariance and expresses the relationship between the returns of two assets in terms of both direction and strength.
    *   The correlation is much easier to interpret since it is standardized and takes values between -1 and +1.
    $$\rho_{i,j} = \frac{cov(r_i, r_j)}{\sigma_i \sigma_j}$$
*   In our example,
    *   $Cov(r_A, r_B) = -0,000414$, $\sigma_A = \%1,70$ and $\sigma_B = \%2,54$
    $$\rho_{A,B} = \frac{-0,000414}{0.017 \times 0.0254} = -0,9588$$

## Portfolio Risk
*   For a two-asset portfolio:
    $$\sigma^2(r_p) = w_1^2 \times \sigma^2(r_1) + w_2^2 \times \sigma^2(r_2) + 2 \times w_1w_2Cov(r_1, r_2)$$

| $r_A$          | 10.10%     | $r_B$          | 9.40%      | Cov($r_A$, $r_B$) | -0.000414  |
| :------------- | :--------- | :------------- | :--------- | :---------------- | :--------- |
| $\sigma_A$     | 1.70%      | $\sigma_B$     | 2.54%      |                   |            |
| $\sigma_A^2$   | 0.000289   | $\sigma_B^2$   | 0.00064516 |                   |            |

| $W_A$ | $W_B$ | $r_p$    | $\sigma_p^2$ | $\sigma_p$ |
| :---- | :---- | :------- | :----------- | :--------- |
| 100%  | 0%    | 10.100%  | 0.000289     | 1.70%      |
| 90%   | 10%   | 10.030%  | 0.000166     | 1.29%      |
| 80%   | 20%   | 9.960%   | 0.000078     | 0.88%      |
| 70%   | 30%   | 9.890%   | 0.000026     | 0.51%      |
| 60%   | 40%   | 9.820%   | 0.000009     | 0.29%      |
| 50%   | 50%   | 9.750%   | 0.000027     | 0.52%      |
| 40%   | 60%   | 9.680%   | 0.000080     | 0.89%      |
| 30%   | 70%   | 9.610%   | 0.000168     | 1.30%      |
| 20%   | 80%   | 9.540%   | 0.000292     | 1.71%      |
| 10%   | 90%   | 9.470%   | 0.000451     | 2.12%      |
| 0%    | 100%  | 9.400%   | 0.000645     | 2.54%      |

Image: Portfolio Standard Deviation vs. Weight of Asset A chart.

## Portfolio Risk
*   Large portfolio variance
    $$E(r_p) = \sum_{i=1}^n w_iE(r_i)$$
    $$\sigma_p^2 = \sum_{i=1}^n \sum_{j=1}^n w_iw_j Cov(r_i, r_j)$$
*   Diversification with an equally weighted portfolio
    $$\sigma_p^2 = \sum_{i=1}^n \frac{1}{n} \sigma_i^2 + \sum_{j=1}^n \sum_{i=1, j \ne i}^n \frac{1}{n^2} Cov(r_i, r_j)$$
    
    Variance terms ($n$)
    Covariance terms ($n(n-1)$)

Image: Portfolio Volatility vs. Number of Stocks chart, illustrating elimination of diversifiable risk and correlated (market) risk.

## Opportunity Set of Risky Assets
*   Minimum-variance frontier shows the risk-return opportunities available to the investor.
*   Efficient frontier
    *   There is an efficient portfolio for each risk level.
    *   Portfolios on the efficient frontier represent trade-offs in terms of risk and return.

| $r_A$          | 10.10%     | $r_B$          | 9.40%      | Cov($r_A$, $r_B$) | -0.000414  |
| :------------- | :--------- | :------------- | :--------- | :---------------- | :--------- |
| $\sigma_A$     | 1.70%      | $\sigma_B$     | 2.54%      |                   |            |
| $\sigma_A^2$   | 0.000289   | $\sigma_B^2$   | 0.00064516 |                   |            |

| $W_A$ | $W_B$ | $r_p$    | $\sigma_p^2$ | $\sigma_p$ |
| :---- | :---- | :------- | :----------- | :--------- |
| 100%  | 0%    | 10.100%  | 0.000289     | 1.70%      |
| 90%   | 10%   | 10.030%  | 0.000166     | 1.29%      |
| 80%   | 20%   | 9.960%   | 0.000078     | 0.88%      |
| 70%   | 30%   | 9.890%   | 0.000026     | 0.51%      |
| 60%   | 40%   | 9.820%   | 0.000009     | 0.29%      |
| 50%   | 50%   | 9.750%   | 0.000027     | 0.52%      |
| 40%   | 60%   | 9.680%   | 0.000080     | 0.89%      |
| 30%   | 70%   | 9.610%   | 0.000168     | 1.30%      |
| 20%   | 80%   | 9.540%   | 0.000292     | 1.71%      |
| 10%   | 90%   | 9.470%   | 0.000451     | 2.12%      |
| 0%    | 100%  | 9.400%   | 0.000645     | 2.54%      |

Image: Efficient Frontier: Portfolio Expected Return vs. Portfolio Standard Deviation chart.

## What is next?
*   Portfolio Theory and Practice II
    *   Readings: Ch. 7
*   Suggested Problems
    *   Chapter 5: 7, 13
    *   Chapter 5 CFA Problems: 1, 2, 3, 4, 5, 6.
    *   Chapter 6: 4, 13, 14, 15, 16, 17, 18.
    *   Chapter 6 CFA Problems: 1, 2, 3, 8
```