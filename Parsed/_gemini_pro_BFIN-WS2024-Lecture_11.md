```markdown
# Investments Finance 2 - BFIN

## Outline
* Derivatives III
  * Binomial Option Pricing Model
  * Black-Scholes Option Pricing Model

## Binomial Option Pricing Model
* A 3-month call option on the stock has a strike price of 21. Risk-free rate is 12%.

```
Stock price = $20
Option Price=?

Stock Price = $22
Option Price = $1

Stock Price = $18
Option Price = $0
```

## Binomial Option Pricing Model
* Consider the portfolio: long $\Delta$ shares, short 1 call option

```
22Δ - 1
     \
      \  Portfolio is riskless when
       \
        \   22Δ – 1 = 18 Δ
         \  Δ = 0.25
          \
           18Δ
```

* The riskless portfolio is long 0.25 shares, short 1 call option
* The value of the portfolio in 3 months is $22 \times 0.25 - 1 = 4.50$
* The value of the portfolio today is $4.5e^{-0.12 \times 0.25} = 4.3670$
* The value of the shares is $5.00 (= 0.25 \times 20)$
* The value of the option is $0.633 (= 5.00 - 4.367)$

## Binomial Option Pricing Model
* Value of a security that gives $1 in the up state, nothing in the down state.
  * Let synthetic portfolio have $\Delta$ units of stock and B in bonds.

$$
S_0 \quad \begin{array}{l} \nearrow \Delta S_0 u + Br \\ f_u = 1 \end{array} \quad \implies \begin{array}{l} f_u = 1 = \Delta S_0 u + Br \\ f_d = 0 = \Delta S_0 d + Br \end{array} \quad \implies \begin{array}{l} \Delta = \frac{1}{S_0(u - d)} \\ B = \frac{-d}{r(u - d)} \end{array}
$$
$$
f_0 \quad \begin{array}{l} \searrow \Delta S_0 d + Br \\ f_d = 0 \end{array}
$$

  * Then, the cost of replicating portfolio is
    $$ \Delta S_0 + B = P_u = \frac{r-d}{r(u-d)} $$

* Value of a security that gives nothing in the up state, $1 in the down state.
$$
\begin{array}{l} f_u = 0 = \Delta S_0 u + Br \\ f_d = 1 = \Delta S_0 d + Br \end{array} \quad \implies \begin{array}{l} \Delta = \frac{-1}{S_0(u - d)} \\ B = \frac{u}{r(u - d)} \end{array} \quad \implies \Delta S_0 + B = P_d = \frac{u-r}{r(u-d)}
$$

* u, d and r and "1 plus rate of return."

## Binomial Option Pricing Model
* Note that buying 1 u-security and 1 d-security gives you $1 for certain. Therefore,
$$ P_u + P_d = 1/r \implies \frac{r-d}{r(u-d)} + \frac{u-r}{r(u-d)} = 1/r \implies \underbrace{\frac{r-d}{u-d}}_{P_u} + \underbrace{\frac{u-r}{u-d}}_{P_d} = 1 $$

* The parameters $p_u$ and $p_d$ should be interpreted as the probability of an up and down movement in a risk-neutral world.
* In a risk-neutral world, the expected return on a stock (or any other investment) is the risk-free rate.
$$ E(S_T) = p_u S_0 u + (1 - p_u)S_0 d \implies E(S_T) = p_u S_0 (u - d) + S_0 d \implies E(S_T) = S_0 r $$

* Risk-neutral valuation provides a very important general result in the pricing of derivatives.
  * It states that, when we assume the world is risk-neutral, we get the right price for a derivative in all worlds, not just in a risk-neutral one.
  * Results are true regardless of the assumptions we make about the evolution of the stock price.
  * To apply risk-neutral valuation to the pricing of a derivative,
    * First calculate what the probabilities of different outcomes would be if the world were risk-neutral.
    * Then, calculate the expected payoff from the derivative and discount that expected payoff at the risk-free rate of interest.

## Binomial Option Pricing Model
* Consider a European call option that expires in one period and has an exercise price of $50. Assume that the stock price today is equal to $50. In one period, the stock price will either rise by $10 or fall by $10. The one-period risk-free rate is 6%.

$$
\begin{array}{ll}
S_0 = 50 \\ f_0
\end{array} \quad \begin{array}{l} \nearrow S_u = 60 \\ f_u = 10 \end{array} \quad \begin{array}{ll} u = 60/50 = 1.20 \\ d = 40/50 = 0.80 \end{array} \quad \begin{array}{l} f_u = 10 = \Delta S_0 u + Br \\ f_d = 0 = \Delta S_0 d + Br \end{array} \quad \begin{array}{l} \Delta = \frac{10}{S_0(u - d)} = 0.50 \\ B = \frac{-d f_u}{r(u - d)} = -18.868 \end{array}
$$
$$
\begin{array}{l} \searrow S_d = 40 \\ f_d = 0 \end{array}
$$

  * The replicating portfolio is long 0.50 shares, short 1 call option, borrows 18.868 for financing.

$$ \Delta S_0 + B = P_u = 0.50 \times 50 + (-18.868) = \$6.132 $$
$$ \Delta S_0 + B = P_u = \frac{(r-d)f_u}{r(u-d)} = \frac{10(1.06-0.80)}{1.06(1.20-0.80)} = \$6.132 $$
$$ p_u = \frac{r-d}{u-d} = 0.65 $$
$$ f_0 = [p_u f_u + (1 - p_u)f_d]r^{-T} = [0.65 \times 10 + (1 - 0.65) \times 0](1.06)^{-1} = \$6.132 $$

## Binomial Option Pricing Model
* The current price of Estelle Corporation stock is $25. In the next year, the stock price will either go up by 20% or go down by 20%. The stock pays no dividends. The one-year risk-free interest rate is 6%. Using the Binomial Model, calculate the price of a one-year put option on Estelle stock with a strike price of $25.

$$
\begin{array}{ll}
S_0 = 25 \\ f_0
\end{array} \quad \begin{array}{l} \nearrow S_u = 30 \\ f_u = 0 \end{array} \quad \begin{array}{ll} u = 1.20 \\ d = 0.80 \end{array} \quad \begin{array}{l} f_u = 0 = \Delta S_0 u + Br \\ f_d = 5 = \Delta S_0 d + Br \end{array} \quad \begin{array}{l} \Delta = \frac{-1 f_d}{S_0(u - d)} = -0.50 \\ B = \frac{u f_d}{r(u - d)} = +14.15 \end{array}
$$
$$
\begin{array}{l} \searrow S_d = 20 \\ f_d = 5 \end{array}
$$

  * The replicating portfolio is short 0.50 shares, long 1 put option, lends 14.15 for financing.

$$ \Delta S_0 + B = P_d = -0.50 \times 25 + 14.15 = \$1.65 $$
$$ p_d = \frac{u-r}{u-d} = 0.35 $$
$$ f_0 = [(1-p_d)f_u + p_d f_d](1+r)^{-T} = [(1 - 0.65) \times 0 + 0.35 \times 5](1.06)^{-1} = \$1.65 $$

## Binomial Option Pricing Model
* Suppose a stock is currently trading for $60, and in one period will either go up by 20% or fall by 10%. If the one-period risk-free rate is 3%, what is the price of a European put option that expires in one period and has an exercise price of $60?

$$
\begin{array}{ll}
S_0 = 60 \\ f_0
\end{array} \quad \begin{array}{l} \nearrow S_u = 72 \\ f_u = 0 \end{array} \quad \begin{array}{ll} u = 1.20 \\ d = 0.90 \end{array} \quad \begin{array}{l} f_u = 0 = \Delta S_0 u + Br \\ f_d = 6 = \Delta S_0 d + Br \end{array} \quad \begin{array}{l} \Delta = \frac{-1 f_d}{S_0(u - d)} = -0.333 \\ B = \frac{u f_d}{r(u - d)} = +23.30 \end{array}
$$
$$
\begin{array}{l} \searrow S_d = 54 \\ f_d = 6 \end{array}
$$

  * The replicating portfolio is short 0.333 shares, long 1 put option, lends 23.30 for financing.

$$ \Delta S_0 + B = P_d = -0.333 \times 60 + 23.30 = \$3.32 $$
$$ p_d = \frac{u-r}{u-d} = 0.567 $$
$$ f_0 = [(1-p_d)f_u + p_d f_d](1+r)^{-T} = [(1 - 0.567) \times 0 + 0.567 \times 6](1.03)^{-1} = \$3.30 $$

## Binomial Option Pricing Model
* We valued of a security that gives $1 in the up state, nothing in the down state.
* More generalized version would be a security that pays $f_u$ in the up state and $f_d$ in the down state.
  * Let synthetic portfolio have $\Delta$ units of stock and B in bonds.

$$
\begin{array}{ll}
S_0 \\ f_0
\end{array} \quad \begin{array}{l} \nearrow \Delta S_0 u + Br \\ f_u \end{array} \quad \implies \begin{array}{l} f_u = \Delta S_0 u + Br \\ f_d = \Delta S_0 d + Br \end{array} \quad \implies \begin{array}{l} \Delta = \frac{f_u - f_d}{S_0(u - d)} \\ B = \frac{u f_d - d f_u}{r(u - d)} \end{array}
$$
$$
\begin{array}{l} \searrow \Delta S_0 d + Br \\ f_d \end{array}
$$

  * Then, the cost of replicating portfolio is
    $$ \Delta S_0 + B = P_0 = \frac{(r-d)f_u - (r-u)f_d}{r(u-d)} $$

* Suppose a stock is currently trading for $60, and in one period will either go up by 20% or fall by 10%. If the one-period risk-free rate is 3%, what is the price of a European put option that expires in one period and has an exercise price of $60?

$$ \Delta = \frac{f_u - f_d}{S_0(u-d)} = \frac{0-6}{60(1.2-0.90)} = -0.333 $$
$$ B = \frac{u f_d - d f_u}{r(u-d)} = \frac{1.20 \times 6 - 0.90 \times 0}{1.03(1.20 - 0.90)} = \$23.30 $$
$$ \Delta S_0 + B = P_0 = \frac{(r-d)f_u - (r-u)f_d}{r(u-d)} = \frac{(1.03-0.90) \times 0 - (1.03-1.20) \times 6}{1.03(1.20-0.90)} = \$3.30 $$

## Binomial Option Pricing Model
* Eagletron's current stock price is $10. Suppose that over the current year, the stock price will either increase by 100% or decrease by 50%. Also, the risk-free rate is 25% (EAR).
  * What is the value today of a one-year at-the-money European put option on Eagletron stock?
  * What is the value today of a one-year at-the-money European call option on Eagletron stock?
  * What is the value today of a one-year European put option on Eagletron stock with a strike price of $20?
  * Suppose the put options in parts a and c could either be exercised immediately, or in one year. What would their values be in this case?

$$ f_u = \max(K - S_u, 0) = \max(10 - 20, 0) = 0 $$
$$ f_d = \max(K - S_d, 0) = \max(10 - 5, 0) = 5 $$
$$ \Delta S_0 + B = P_0 = \frac{(r-d)f_u - (r-u)f_d}{r(u-d)} = \frac{(1.25-0.50) \times 5 - (1.25-2.00) \times 0}{1.25(2.00-0.50)} = \$2.00 $$
$$ f_u = \max(S_u - K, 0) = \max(20 - 10, 0) = 10 $$
$$ f_d = \max(S_d - K, 0) = \max(5 - 10, 0) = 0 $$
$$ \Delta S_0 + B = P_0 = \frac{(r-d)f_u - (r-u)f_d}{r(u-d)} = \frac{(1.25-0.50) \times 0 - (1.25-2.00) \times 10}{1.25(2.00-0.50)} = \$4.00 $$
$$ f_u = \max(K - S_u, 0) = \max(20 - 20, 0) = 0 $$
$$ f_d = \max(K - S_d, 0) = \max(20 - 5, 0) = 15 $$
$$ \Delta S_0 + B = P_0 = \frac{(r-d)f_u - (r-u)f_d}{r(u-d)} = \frac{(1.25-0.50) \times 15 - (1.25-2.00) \times 0}{1.25(2.00-0.50)} = \$6.00 $$

## Binomial Option Pricing Model
* A 6-month call option on the stock has a strike price of 21. Risk-free rate is 12%. Stock goes up or down 10% for 2 periods (Each period is 3 months).

*(Diagram of a 2-period binomial tree showing stock prices and option payoffs)*

$$ \Delta S_0 + B = P_1^u = \frac{(r-d)f_{uu} - (r-u)f_{ud}}{r(u-d)} = \frac{(1.03-0.90) \times 3.2 - (1.03 - 1.10) \times 0}{1.03(1.10 - 0.90)} = \$2.02 $$
$$ \Delta S_0 + B = P_0 = \frac{(r-d)f_u - (r-u)f_d}{r(u-d)} = \frac{(1.03-0.90) \times 2.02 - (1.03 - 1.10) \times 0}{1.03(1.10 - 0.90)} = \$1.27 $$

## Binomial Option Pricing Model
* The current price of Natasha Corporation stock is $6. In each of the next two years, this stock price can either go up by $2.50 or go down by $2. The stock pays no dividends. The one-year risk-free interest rate is 3% and will remain constant. Using the Binomial Model, calculate the price of a two-year call option on Natasha stock with a strike price of $7.

*(Diagram of a 2-period binomial tree showing stock prices and call option values)*

$$ \Delta S_0 + B = P_1^u = \frac{(r-d)f_{uu} - (r-u)f_{ud}}{r(u-d)} = \frac{(1.03-0.7647) \times 4 - (1.03 - 1.2941) \times 0}{1.03(1.2941 - 0.7647)} = \$1.9461 $$
$$ \Delta S_0 + B = P_0 = \frac{(r-d)f_u - (r-u)f_d}{r(u-d)} = \frac{(1.03-0.6667) \times 1.9461 - (1.03 - 1.4167) \times 0}{1.03(1.4167 - 0.6667)} = \$0.9152 $$

## Binomial Option Pricing Model
* The current price of Natasha Corporation stock is $6. In each of the next two years, this stock price can either go up by $2.50 or go down by $2. The stock pays no dividends. The one-year risk-free interest rate is 3% and will remain constant. Using the Binomial Model, calculate the price of a two-year put option on Natasha stock with a strike price of $7.

*(Diagram of a 2-period binomial tree showing stock prices and put option values)*

$$ \Delta S_0 + B = P_1^d = \frac{(r-d)f_{du} - (r-u)f_{dd}}{r(u-d)} = \frac{(1.03-0.50) \times 0.50 - (1.03 - 1.625) \times 5}{1.03(1.625 - 0.50)} = \$2.7961 $$
$$ \Delta S_0 + B = P_1^u = \frac{(r-d)f_{uu} - (r-u)f_{ud}}{r(u-d)} = \frac{(1.03-0.7647) \times 0 - (1.03 - 1.2941) \times 0.50}{1.03(1.2941 - 0.7647)} = \$0.2422 $$
$$ \Delta S_0 + B = P_0 = \frac{(r-d)f_u - (r-u)f_d}{r(u-d)} = \frac{(1.03-0.6667) \times 0.2422 - (1.03 - 1.4167) \times 2.7961}{1.03(1.4167 - 0.6667)} = \$1.514 $$

## Binomial Option Pricing Model
* European put option with a strike price of 52.
* Either up 20% or down 20%. Each time step is 1 year, r=5%.

*(Diagram of a 2-period binomial tree with stock prices and European put values)*

$$ P_1^d = \frac{(1.05 - 0.80) \times 4 - (1.05 - 1.20) \times 20}{1.05(1.20 - 0.80)} = \$9.524 $$
$$ P_1^u = \frac{(1.05 - 0.80) \times 0 - (1.05 - 1.20) \times 4}{1.05(1.20 - 0.80)} = \$1.429 $$
$$ P_0 = \frac{(1.05 - 0.80) \times 1.429 - (1.05 - 1.20) \times 9.524}{1.05(1.20 - 0.80)} = \$4.25 $$

* American put option with a strike price of 52.
* Either up 20% or down 20%. Each time step is 1 year, r=5%.

*(Diagram of a 2-period binomial tree with stock prices and American put values)*

$$ P_1^d = \frac{(1.05 - 0.80) \times 4 - (1.05 - 1.20) \times 20}{1.05(1.20 - 0.80)} = \$9.524 < (52 - 40) $$
$$ P_1^u = \frac{(1.05 - 0.80) \times 0 - (1.05 - 1.20) \times 4}{1.05(1.20 - 0.80)} = \$1.429 $$
$$ P_0 = \frac{(1.05 - 0.80) \times 1.429 - (1.05 - 1.20) \times 12}{1.05(1.20 - 0.80)} = \$5.14 $$

## Black-Scholes Option Pricing Model
* Key assumptions
  * There are no arbitrage opportunities.
  * Underlying asset is a traded security, and investors can trade continuously.
  * The option to be priced is European.
  * Constant volatility (equal u and d moves through the tree), with no jumps.
  * No transaction costs or taxes, securities perfectly divisible, no portfolio restrictions, investors are price-takers.
* Continuous trading assumption
  * When markets are open, we can trade as we wish, so it is a good approximation.
  * But markets do close, so continuous trading is not ideal.

## Black-Scholes Option Pricing Model
### Black-Scholes Price of a Call Option on a Non-Dividend-Paying Stock
$$ C_t = S_t \times N(d_1) - PV(K) \times N(d_2) \quad \text{where} $$
$$ d_1 = \frac{\ln(S_t/PV(K))}{\sigma\sqrt{T-t}} + \frac{\sigma\sqrt{T-t}}{2} $$
$$ d_2 = d_1 - \sigma\sqrt{T-t} $$

### Black-Scholes Price of a Put Option on a Non-Dividend-Paying Stock
$$ P_t = PV(K)[1 - N(d_2)] - S_t[1 - N(d_1)] $$

* Default notation
  * $S_t$: Value of the underlying asset at date t;
  * $K$: Strike price of the option;
  * $r_f$: Risk-free rate (annual terms);
  * $\sigma$: Volatility (in annual terms), i.e. squared root of the variance;
  * $T$: Maturity, so at date t, $T-t$ is time to maturity.
  * $N(d)$: The cumulative normal distribution

## Black-Scholes Option Pricing Model
### Black-Scholes Price of a Call Option on a Non-Dividend-Paying Stock
$$ C_t = S_t \times N(d_1) - PV(K) \times N(d_2) \quad \text{where} $$
$$ d_1 = \frac{\ln(S_t/PV(K))}{\sigma\sqrt{T-t}} + \frac{\sigma\sqrt{T-t}}{2} $$
$$ d_2 = d_1 - \sigma\sqrt{T-t} $$

### Black-Scholes Price of a Put Option on a Non-Dividend-Paying Stock
$$ P_t = PV(K)[1 - N(d_2)] - S_t[1 - N(d_1)] $$

* The value of a call is a weighted difference of the present value of its potential benefits, $S_t$, and the present value of its potential costs $PV(K)$ where the weights $N(d_1)$ and $N(d_1 - \sigma\sqrt{T-t})$ are in $(0, 1)$.
* The value of a put is a weighted difference of the present value of its potential costs $PV(K)$, and the present value of its potential benefits, $S_t$, where the weights $[1 - N(d_2)]$ and $[1 - N(d_1)]$ are in $(0, 1)$.

$$ C_t = \underbrace{S_t \times N(d_1)}_{\Delta} - \underbrace{PV(K) \times N(d_2)}_{\text{Borrowing}} \implies C_t = \text{Asset Price} \times \text{Delta} + \text{Cash Position} $$

## Black-Scholes Option Pricing Model
*(Diagram of a normal distribution curve with N(d) shaded)*

* The cumulative normal distribution [$N(d)$]
  * The probability that a normally distributed random variable will take on a value less than d.
  * Equal to the area under the normal distribution to the left of the point d.
  * $N(d)$ has a minimum value of 0 and a maximum value of 1.
  * Can be calculated in Excel using the function NORMSDIST(d).

$$ d_1 = \frac{\ln(S_t/PV(K))}{\sigma\sqrt{T-t}} + \frac{\sigma\sqrt{T-t}}{2} $$
$$ d_2 = d_1 - \sigma\sqrt{T-t} $$

* Volatility (standard deviation) follows the squared-root rule.
  * Monthly volatility is $\sigma_m$, then the annual volatility is $\sigma_a = \sqrt{12}\sigma_m$
  * Weekly volatility is $\sigma_w$, then the annual volatility is $\sigma_a = \sqrt{52}\sigma_w$
  * Daily volatility is $\sigma_d$, then the annual volatility is $\sigma_a = \sqrt{250}\sigma_d$

## Black-Scholes Option Pricing Model
*(Graph: Black-Scholes call option price)*
*(Graph: Black-Scholes put option price)*

## Black-Scholes Option Pricing Model
* Only non-observable variable in Black-Scholes Model is volatility($\sigma$).
  * One option is to use historical data on daily stock returns to estimate the volatility of the stock over the past several months.
  * Implied volatility
    * The Black-Scholes formula can be expressed as $C_t = C(S_t, K, r_f, T, \sigma)$
    * If we know the price of a given option $C_t$, we can solve the Black-Scholes formula for $\sigma$.
    * In this case, $\sigma$ is called the implied volatility of the option.

## Black-Scholes Option Pricing Model
*(Graph: VIX (%) over time, showing various financial crises)*

## Black-Scholes Option Pricing Model
$$ C_t = \underbrace{S_t \times N(d_1)}_{\Delta} - \underbrace{PV(K) \times N(d_2)}_{\text{Borrowing}} $$
$$ P_t = \underbrace{PV(K) \times [1 - N(d_2)]}_{\text{Lending}} - \underbrace{[1 - N(d_1)]}_{\Delta} \times S_t $$

* The option delta, $\Delta$, is the change in the price of the option given a 1-unit change in the price of the stock.
  * Because $\Delta$ is always less than 1, the change in the call price is always less than the change in the stock price.
  * When the price of the underlying asset changes, $\Delta$ also changes.
  * If we can update our portfolio continuously, we can replicate an option on the stock by constantly adjusting our portfolio to remain on a line that is tangent to the value of the option.

*(Graph: Black-Scholes Option Value, Intrinsic Value, Replicating Portfolio)*

## Black-Scholes Option Pricing Model
* Risk and Return of an Option
$$ \beta_{Option} = \frac{S_t \Delta}{S_t \Delta + B} \beta_S + \frac{B}{S_t \Delta + B} \beta_B $$
$$ \text{Since } \beta_B = 0, \quad \beta_{Option} = \frac{S_t \Delta}{S_t \Delta + B} \beta_S $$
$$ \frac{S_t \Delta}{S_t \Delta + B} \text{ is the options leverage ratio.} $$

One-year options on a stock with a 30% volatility, given a risk-free interest rate of 5%.

*(Graph: Leverage Ratio vs Stock Price)*
*(Graph: Expected Return vs Beta)*

## Black-Scholes Option Pricing Model
* Roslin Robotics stock has a volatility of 30% and a current stock price of $60 per share. Roslin pays no dividends. The risk-free interest is 5%. Determine the Black-Scholes value of a one-year, at-the-money call option on Roslin stock.

$$ C_t = S_t \times N(d_1) - PV(K) \times N(d_2) $$
$$ d_1 = \frac{\ln(S_t/PV(K))}{\sigma\sqrt{T-t}} + \frac{\sigma\sqrt{T-t}}{2} = \frac{\ln(60/ (60 \times (1+0.05)^{-1}))}{0.30\sqrt{1}} + \frac{0.30\sqrt{1}}{2} = 0.312634 $$
$$ N(d_1) = 0.622721 $$
$$ d_2 = d_1 - \sigma\sqrt{T-t} = 0.312634 - 0.30 = 0.012634 $$
$$ N(d_2) = 0.50504 $$
$$ C_t = S_t \times N(d_1) - PV(K) \times N(d_2) = 60 \times 0.622721 - 60 \times (1+0.05)^{-1} \times 0.50504 = \$8.5038 $$

  * Suppose the call option is not available for trade in the market. You would like to replicate a long position in call option. What portfolio should you hold today?
$$ C_t = \underbrace{S_t \times N(d_1)}_{\Delta} - \underbrace{PV(K) \times N(d_2)}_{\text{Borrowing}} $$
$$ \Delta = N(d_1) = 0.622721 $$
$$ \Delta S_t = 0.622721 \times 60 = \$37.3633 $$
$$ B = -PV(K) \times N(d_2) = - (60 \times (1+0.05)^{-1} \times 0.50504) = -28.8594 $$

## Black-Scholes Option Pricing Model
* Rebecca is interested in purchasing a European call on a hot new stock, Up, Inc. The call has a strike price of $100 and expires in 90 days. The current price of Up stock is $120, and the stock has a standard deviation of 40% per year. The risk-free interest rate is 6.18% per year.
  * Using the Black-Scholes formula, compute the price of the call.

$$ d_1 = \frac{\ln(S_t/PV(K))}{\sigma\sqrt{T-t}} + \frac{\sigma\sqrt{T-t}}{2} = \frac{\ln(120/(100 \times (1.0618)^{-0.25}))}{0.40\sqrt{0.25}} + \frac{0.40\sqrt{0.25}}{2} = 1.0866 $$
$$ N(d_1) = 0.8614 $$
$$ d_2 = d_1 - \sigma\sqrt{T-t} = 1.0866 - 0.40\sqrt{0.25} = 0.8866 $$
$$ N(d_2) = 0.8123 $$
$$ C_t = S_t \times N(d_1) - PV(K) \times N(d_2) = 120 \times 0.8614 - 100 \times (1.0618)^{-0.25} \times 0.8123 = \$23.34 $$

  * Use put-call parity to compute the price of the put with the same strike and expiration date.
$$ P_t = C_t - S_t + K(1+r_f)^{-(T-t)} = 23.34 - 120 + 100(1 + 0.0618)^{-0.25} = \$1.8520 $$

## Black-Scholes Option Pricing Model
* Consider an at-the-money put option on AGE Inc stock that expires in 6 months. The stock of AGE Inc is currently trading at $5, and you estimate the volatility of AGE Inc to be 50% per year and its beta is 0.90. The short-term risk-free rate of interest is 4% per year.
  * What is the put option's leverage ratio?
  * What is the beta of the put option?
  * If the expected risk premium of the market is 6%, what is the expected return of the put option based on the CAPM?
  * Given its expected return, why would an investor buy a put option?

$$ N(d_1) = 0.5918 $$
$$ N(d_2) = 0.4517 $$
$$ P_t = PV(K)[1 - N(d_2)] - S_t[1 - N(d_1)] $$
$$ P_t = 5 \times (1.04)^{-0.50} [1 - 0.4517] - 5[1 - 0.5918] = 0.6473 $$
$$ \Delta = (-(1 - N(d_1))) = -(1 - 0.5918) = -0.4082 $$
$$ P_t = \underbrace{PV(K) \times [1 - N(d_2)]}_{\text{Lending}} - \underbrace{[1 - N(d_1)]}_{\Delta} \times S_t $$
$$ B = 5 \times (1.04)^{-0.50} \times [1 - 0.4517] = 2.6883 $$
$$ \text{Option Leverage Ratio} = \frac{S_t \Delta}{S_t \Delta + B} = \frac{5 \times (-0.4082)}{5 \times (-0.4082) + 2.6883} = -3.15 $$
$$ \beta_{Option} = -3.15 \times 0.90 = -2.84 $$
$$ E[R_{option}] = r_f + \beta_{option}(E[R_{Mkt}] - r_f) $$
$$ E[R_{option}] = 0.04 + (-2.84)(0.06) = -13.04\% $$

## Black-Scholes Option Pricing Model
* A stock is currently priced at $84. The stock will either increase or decrease by 17 percent over the next year. There is a call option on the stock with a strike price of $80 and one year until expiration. If the risk-free rate is 8 percent, what is the risk-neutral value of the call option?

$$ C_{t=1}^u = \max(S_t^u - K, 0) = \max(84 \times 1.17 - 80, 0) = \$18.28 $$
$$ C_{t=1}^d = \max(S_t^d - K, 0) = \max(84 \times 0.83 - 80, 0) = \$0 $$
$$ p_u = \frac{r-d}{u-d} = \frac{1.08-0.83}{1.17-0.83} = 0.7353 $$
$$ p_d = \frac{u-r}{u-d} = \frac{1.17-1.08}{1.17-0.83} = 0.2647 $$
$$ C_0 = \frac{p_u \times C_{t=1}^u + p_d \times C_{t=1}^d}{(r)^1} = \frac{0.7353 \times 18.28 + 0.2647 \times 0}{1.08} = \$12.45 $$

## What is next?
* Solutions to all suggested problems
* Final exam on October 25, 2024
* Assignment 2 due by 16:00, October 30
```