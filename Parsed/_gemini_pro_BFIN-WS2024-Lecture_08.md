```markdown
# Investments Finance 2 - BFIN
### Dr. Omer CAYIRLI
### Lecture 8

## Outline
* Multifactor Models
* Arbitrage Pricing Theory

## APT and Multifactor Models of Risk and Return
### Single Factor Model
* Returns on a security come from two sources:
    * Common macro-economic factor
    * Firm specific events
* Possible common macro-economic factors
    * Gross Domestic Product growth
    * Interest rates

$R_i = E(R_i) + \beta_i F + e_i$

### Multifactor Models
* Use more than one factor:
    * Market Return, GDP, Expected Inflation, Interest Rates
* Estimate a beta or factor loading for each factor using multiple regression

$R_i = E(R_i) + \beta_{iGDP}GDP + \beta_{iIR}IR + e_i$

## APT and Multifactor Models of Risk and Return
### Markowitz Mean-variance Portfolio Theory
* Introduced by Harry Markowitz in the 1950
* Foundation of modern portfolio theory
* Mean-variance optimizers (Expected return & variance)
    * Global minimum variance portfolio
    * Efficient portfolios
* There is no natural starting point for the expected return assumptions

### The Capital Asset Pricing Model
* Linear, single period & one factor equilibrium model
* Enables us to generate expected returns for any asset using the systematic risk(Beta), and the market risk premium.
* Relatively strong assumptions

## APT and Multifactor Models of Risk and Return
### The Arbitrage Pricing Theory (APT)
* Models the expected return of a financial asset as a function of various macroeconomic factors or theoretical market indexes.
* Multifactor models

### Multifactor Asset Pricing Models
* Fama-French Models (Three-factor & five-factor models)
* Mostly based on the previous empirical findings regarding return anomalies.
* Factor-augmented versions of the CAPM but built on the APT.

### CAPM vs. APT & Multifactor models
* CAPM – Homogeneous expectations, mean-variance preferences, single factor, market.
* APT – No assumption about expectations or investor risk preferences, does not explicitly state what the factors are.

## APT and Multifactor Models of Risk and Return
### CAPM
* There is one risk premium, which can be captured by the market portfolio.

### APT & Multifactor models
* There are other risk premia than the market risk premium.

* It is all about whether $\alpha = 0$ or not.

## APT and Multifactor Models of Risk and Return
### The Arbitrage Pricing Theory (APT)
* Arbitrage occurs if there is a zero investment portfolio with a sure profit
* No investment -> Investors create large positions to obtain large profits
* All investors will want an infinite position in the risk-free arbitrage portfolio
* In efficient markets, profitable arbitrage opportunities will quickly disappear

### The Law of One Price:
* Enforced by arbitrageurs: If they observe a violation they will engage in arbitrage activity
* This bids up (down) the price where it is low (high) until the arbitrage opportunity is eliminated

## APT and Multifactor Models of Risk and Return
$R_P = E(R_P) + \beta_P F + e_P$ where $F = \text{SystematicRisk}$

$E(R_P) = \sum w_i E(R_i)$

$\beta_P = \sum w_i \beta_i$

$e_P = \sum w_i e_i$

### For a well-diversified portfolio,
* $e_P \to 0$ as the number of securities increases and weights decrease

## APT and Multifactor Models of Risk and Return
**Panel A, Well-diversified portfolio**

Excess Return (%)

A

10

0

F

A

**Panel B, Single stock (S)**

Excess Return (%)

S

10

0

F

B

## APT and Multifactor Models of Risk and Return
### No-Arbitrage Equation of APT
$E(R_P) = \beta_P E(R_M)$

* Applies to well-diversified portfolios
* Establishes that the SML of CAPM applies to well-diversified portfolios

| APT                                                                                              | CAPM                                                                                                                                                             |
| :----------------------------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| * Assumes a well-diversified portfolio, but residual risk is still a factor                      | * Model is based on an inherently unobservable "market" portfolio                                                                                              |
| * Does not assume investors are mean-variance optimizers                                         | * Rests on mean-variance efficiency. The actions of many small investors restore CAPM equilibrium                                                                |
| * Uses an observable market index                                                                |                                                                                                                                                                  |
| * Reveals arbitrage opportunities                                                                |                                                                                                                                                                  |

## APT and Multifactor Models of Risk and Return
* Before CAPM
    $E[R_i] - R_f = \alpha_i$

* With CAPM
    $E[R_i] - R_f = \beta^m (E[R_m] - R_f)$

* Alpha is still there!
    $E[R_i] - R_f = \alpha_i + \beta^m (E[R_m] - R_f)$

* Fama and French (1992)
    $E[R_i] - R_f = \beta^m (E[R_m] - R_f) + \beta^{smb}[R_{smb}] + \beta^{hml} [R_{hml}]$

* Carhart (1997)
    $E[R_i] - R_f = \beta^m (E[R_m] - R_f) + \beta^{smb} [R_{smb}] + \beta^{hml} [R_{hml}] + \beta^{wml}[R_{wml}]$

* Fama and French (2015)
    $E[R_i] - R_f = \beta^m (E[R_m] - R_f) + \beta^{smb} [R_{smb}] + \beta^{hml} [R_{hml}] + \beta^{rmw} [R_{rmw}] + \beta^{cma}[R_{cma}]$

## APT and Multifactor Models of Risk and Return
### Multifactor APT
* Use of more than a single systematic factor
* Requires formation of factor portfolios
* What factors?
    * Factors that are important to the performance of the general economy
    * What about firm characteristics?

### The multifactor APT is similar to the one-factor case
$R_i = E(R_i) + \beta_{i1}F_1 + \beta_{i2}F_2 + e_i$

### Track with diversified factor portfolios:
* $\beta=1$ for one of the factors and $0$ for all other factors
* The factor portfolios track a particular source of macroeconomic risk, but are uncorrelated with other sources of risk

## APT and Multifactor Models of Risk and Return
### Fama-French Three-Factor Model
$R_{it} = \alpha_i + \beta_{iM}R_{Mt} + \beta_{iSMB}SMB_t + \beta_{iHML}HML_t + e_{it}$

* Are these firm characteristics correlated with actual systematic risk factors?

### Fama and French (1992) find that firm characteristics other than beta help explain returns
* Firm size (ME = market value of equity)
* Book-to-market ratio (B/M = book value of equity / market value of equity)
* Methodology:
    * Sort all stocks by size (ME) and determine decile breakpoints for ME
    * Allocate stocks to 10 size portfolios
    * Subdivide each size decile into 10 portfolios on the basis of beta

## APT and Multifactor Models of Risk and Return
### Fama-French Three-Factor Model
* Firm size
    * Average stock returns of small firms are higher than predicted by the CAPM
    * After controlling for size, beta does not explain much of the cross-sectional variation of average returns
* Book-to-market ratio market ratio
    * Firms with higher book-to-market ratios have higher average returns
    * B/M-based portfolios show almost no variation in beta
    * B/M ratio is negatively correlated with size

### What Do We Learn From These Tests?
* Single-factor traditional CAPM does not work?
* Size may or may not be a priced factor
    * Size works in the Fama-French model from 1962 to 1989
    * Size premium disappeared in the 90s
* Book-to-market ratio seems to be a priced factor
    * Value stocks (high B/M stocks) earn higher expected returns than growth stocks (low B/M stocks)
    * Problem is, we don't really know why
* Time variation in risk matters

## Asset pricing in a multifactor setting
### Asset pricing in a multifactor setting
* Raises a critique of multifactor models used in asset pricing literature.
* Mathematically shows that, no matter how many factors are added to the capital asset pricing model (CAPM), beta will always matter.
* Also shows that augmenting factors to the single-factor CAPM requires market risk premiums to be modeled as time varying.
* Offers a fairly simple way to estimate expected excess returns in a multifactor setting without the use of sorting methodologies.

## Asset pricing in a multifactor setting
$E(R_i) = R_f + \beta_i [E(R_M) - R_f]$ for $i=1,...,N$ (Eq. 1) Sharpe-Lintner version of CAPM

* May be written as,
    $E(R_i) = (1 - \beta_i)R_f + \beta_i E(R_M)$ (Eq. 2)

* Sharpe-Lintner's version of CAPM may be manipulated further by subtracting $E(R_M)$ from both sides,
    $E(R_i^{ex}) = (\beta_i - 1)[E(R_M) - R_f]$ (Eq. 3)

* Conveys information on the expected relative performance of asset $i$ compared to the market.
* The only risk factor that does matter in this setting is the systemic component.

## Asset pricing in a multifactor setting
* Assume that there is another factor (X) that is relevant for $E(R_i^{ex})$. Denoting asset $i$'s sensitivity to this factor as $\phi_i$, we can rewrite the pricing equation as follows,
    $E(R_i^{ex}) = (\beta_i - 1)[E(R_M) - R_f] + \phi_i E(X)$ (Eq. 4)

* In this setting,
    * If X is an idiosyncratic factor, it will not be priced; hence, $\phi_i$ will not be different than zero and equation will collapse to a one-factor model.
    * If X is a priced factor, $\phi_i$ will be different than zero and since the market is the sum of individual assets, the market return will also be sensitive to the factor X.

* Then, the expected return on the market portfolio in the period ($t_0, t_1$) may be written as follows where $\phi_M$ represents the market's sensitivity to factor X, and $E(\bar{R}_M)$ is the market risk premium observed at $t_0$.
    $E(R_M) = E(\bar{R}_M) + \phi_M d(E(X))$ (Eq. 5)

* Substituting this into the previous equation for $E(R_M)$ yields the following equation,
    $E(R_i^{ex}) = (\beta_i - 1)[E(\bar{R}_M) + \phi_M d(E(X)) - R_f] + \phi_i E(X)$ (Eq. 6)

## Asset pricing in a multifactor setting
$E(R_i^{ex}) = (\beta_i - 1)[E(\bar{R}_M) + \phi_M d(E(X)) - R_f] + \phi_i E(X)$ (Eq. 6)

* Taking the differential of equation of this equation we have,
    $d(E(R_i^{ex})) = (\beta_i \phi_M - \Phi_M) + \phi_i d(E(X))$ (Eq. 7)
    $d(E(R_i^{ex})) = (\beta_i-1)\phi_M + \phi_i d(E(X))$ (Eq. 8)
* Assuming that $\beta_i$ is the estimated systemic risk of asset $i$ at time $t_0$, and constant.
* Also assume that $\phi_M$ and $\phi_i$ are also constant.

* Follows from the fact that the only source of change in the pricing equation is $E(X)$.

* Conveys that, in a two-factor setting, the expected relative performance of asset $i$ compared to market will be determined by $\beta_i$ at $t=0$, market's sensitivity to factor X ($\phi_M$), and asset $i$'s sensitivity to the factor X ($\phi_i$).

* As long as there is a change in $E(X)$, unless $[(\beta_i-1)\phi_M/\phi_i] = -d(E(X))$ then $d(E(R_i^{ex}))$ will always be different than zero.

## Asset pricing in a multifactor setting
$d(E(R_i^{ex})) = (\beta_i-1)\phi_M + \phi_i d(E(X))$ (Eq. 8)

* When the single-factor CAPM is augmented with a priced factor, the total impact of a change in $E(X)$ on $E(R_i^{ex})$ will be jointly determined by $\beta_i, \phi_M, \phi_i$, and $d(E(X))$.

* For $(\beta_i > 1)$ if both $\phi_M$ and $\phi_i$ have the same sign, then an increase in $E(X)$ will be amplified whereas an impact of a decrease in $E(X)$ will be less than the same amount of increase, suggesting an asymmetric response to the changes in $E(X)$.

* For $(\beta_i < 1)$, the reverse will be true and a decrease in $E(X)$ will have a larger impact on $E(R_i^{ex})$ then the similar amount of increase.

* For $(\beta_i > 1)$ and opposite signs of $\phi_M$ and $\phi_i$, an asymmetric response will be observed such that the effect of decrease will be greater than the same amount of increase. Again, the reverse will be true for $(\beta_i < 1)$.

* Fama and French (1992) argue that if there is a role for beta in average returns, it is likely to be found in a multi-factor model that transforms the flat simple relation between average return and beta into a positively sloped conditional relation. The analyses above clearly provide evidence for not only the conditional relation but also asymmetric responses.

## Asset pricing in a multifactor setting
* It is often neglected that if at least one asset in the market portfolio is sensitive to a priced factor, then the market portfolio should also be sensitive to this factor.

* As the number of assets that are sensitive to a specific factor increases, it is likely for an investor to encounter a set of assets that have varying response profiles to the expected changes to the factor under question.

* Nevertheless, these varying response profiles will always depend on the values of $\beta_i, \phi_M, \phi_i$, and $d(E(X))$.

## Asset pricing in a multifactor setting
* If the second factor is priced, the total change in expected excess return as a response to a change $E(X)$ will be dependent on the beta in addition to $\phi_M$ and $\phi_i$.

* For beta not to matter, $\phi_M$ should not be different than zero and this condition can be satisfied only in two situations:
    * When $\phi$ for all assets is not different than zero, $\phi_M$ will also be zero, which means that factor X is irrelevant.
    * There might be a special case in which $\phi_M$ is zero but more than one asset is sensitive to the factor. In this case, a combination of these assets that are sensitive to factor X should be perfect hedges for each other with respect to factor X. This is the definition of an idiosyncratic risk that can be diversified away and that should not be priced as a risk factor.

* In order to prove that beta does not matter, the necessary assumption is that the expected return on the market portfolio is not sensitive to factor X.

* As long as there is an asset $i$ that is in the market portfolio and sensitive to priced factor X, this necessary condition for proving that beta does not matter cannot be satisfied.

## Asset pricing in a multifactor setting
* We also derive the pricing equation in a three-factor setting.

* Assume that the augmented factors, X and Y, are independent,
    $d(E(R_i^{ex})) = (\beta_i-1)\phi_M + \phi_i d(E(X)) + (\beta_i-1)\gamma_M + \gamma_i d(E(Y))$ (Eq. 9)

* Removing the independence assumption,
    $d(E(R_i^{ex})) = A d(E(X)) + B d(E(Y))$ (Eq. 10)
    where,
    $A = (\beta_i-1)\phi_M + [(\beta_i-1)\gamma_M d(E(Y)) + \phi_i + \gamma_i E(Y)]$ (Eq. 11)
    $B = (\beta_i-1)\phi_M + [(\beta_i-1)\phi_M d(E(X)) + \phi_i E(X) + \gamma_i]$ (Eq. 12)

* The beta will still matter as long as asset $i$ is in the market portfolio and both X and Y are priced factors.

* For a three-factor model, the channel from the priced factors to $E(R_i^{ex})$ becomes more complicated when the additional factors co-vary, but beta is still "alive”.

## Asset pricing in a multifactor setting
* Most striking difference is that when the additional factors are allowed to co-vary, the levels of these factors also become relevant.
    * When the levels of these additional factors are relevant, it is not surprising to obtain significant coefficients using sorting methodologies.
    * Sorting methodologies implicitly treat these variables as conditioning variables and remove some of the heterogeneity.
    * Fama and French (1992) note that the correlation between size and book-to-market equity affects the regressions. However, they argue that the links between size and book-to-market equity should not be exaggerated.

## Asset pricing in a multifactor setting
* Risk-premiums for the size and book-to-market factors as determinants of expected returns are highly likely to be just capturing the conditional impact of another underlying factor.
    * A change in this underlying factor may be inducing changes in the expected returns conditional on the size and/or book-to-market equity.
    * There may be many other factors that impact expected returns in a similar conditional nature.
    * The underlying factor may impact the excess returns conditional on both factors in the three-factor case.
    * Aside from being conditioning variables, size and/or book-to-market equity may also be risk factors at the same time.

* If the size and book-to-market equity factors are aggregating the conditional information from the underlying factors, they will not be time-invariant as long as the conditional-response generating factor(s) are time-varying.

* Also true for the market-risk premia.

## Asset pricing in a multifactor setting
* Beta will always be relevant no matter how many factors are augmented to the single-factor model.

* The multi-factor models that employ additional risk factors should model the market risk-premium in a time-varying fashion since changes in the augmented factor, if priced, will have an impact on the market return as well.

* Our approach also captures conditional impacts which is pertinent to the argument raised by Fama and French (1992) that if there is a role for beta in average returns, it is likely to be found in a multi-factor model that transforms the flat simple relation between average return and beta into a positively sloped conditional relation.
    * For this inherent conditionality to become apparent, it is imperative for researchers to use a specification that takes into account that a change in the priced factor(s) will not only affect individual assets but also the expected market excess returns.

* The developed approach allows estimating the expected excess returns in a multi-factor setting without drawing upon the sorting methodologies.
    * Strongly recommend the use of underlying factors that induce changes in the expected returns, whatever they may be.

## What is next?
### Tutorial Session cont'd (15.10.2024)
### Derivatives I (16.10.2024)
* Introduction to Derivatives
* Futures and Forwards
* Futures, Swaps, and Risk Management
* Reading(s): BKM Ch. 22 & 23
```