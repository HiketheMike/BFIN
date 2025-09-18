```markdown
# Investments Finance 2 - BFIN

Dr. Omer CAYIRLI
Lecture 10

## Outline

*   Derivatives II
    *   Introduction to options
    *   Option Payoffs
    *   Put-Call Parity
    *   Factors Affecting Option Prices

## Introduction to Options

*   Options are an example of a broader class of assets called contingent claims.
    *   A contingent claim is any asset whose future payoff is contingent on the outcome of some uncertain event.
*   A financial option contract gives its owner the right (but not the obligation) to purchase or sell an asset at a fixed price at some future date.
    *   Call options
    *   Put options
    *   Option buyer (holder), Option seller (writer)
    *   Long position (right), short position (obligation)
    *   Option premium: The market price of the option.
        *   Compensates the seller for the risk of loss in the event that the option holder chooses to exercise the option.

## Introduction to Options

*   The price at which the holder buys or sells the underlying asset when the option is exercised is called the strike price or exercise price.
    *   At-the-money: When the exercise price of an option is equal to the current price of the underlying asset.
    *   In-the-money: If the payoff from exercising an option immediately is positive.
    *   Out-of-the-money: If the payoff from exercising the option immediately is negative.
*   American options allow their holders to exercise the option on any date up to and including the expiration date.
*   European options allow their holders to exercise the option only on the expiration date.

## Option Payoffs

Analytical payoffs of a call: $\max(S_T – K, 0)$
Analytical payoffs of a putt: $\max(K – S_T, 0)$

## Option Strategies

*   Protective put positions: long asset and a long put.

| | $S_T \le K$ | $S_T > K$ |
| :------- | :-------- | :-------- |
| Stock | $S_T$ | $S_T$ |
| +Put | $K-S_T$ | 0 |
| Total | $K$ | $S_T$ |

*   Covered call positions: long asset and a short call.

| | $S_T \le K$ | $S_T > K$ |
| :------- | :-------- | :-------- |
| Stock | $S_T$ | $S_T$ |
| -Call | 0 | $-(S_T-K)$ |
| Total | $S_T$ | $K$ |

## Option Strategies

*   Bull spreads: long call $K_1$ and short call $K_2$ with $K_1 < K_2$.

| | $S_T \le K_1$ | $K_1 < S_T \le K_2$ | $S_T \ge K_2$ |
| :-------- | :----------- | :------------------ | :---------- |
| +Call@$K_1$ | 0 | $S_T-K_1$ | $S_T-K_1$ |
| -Call@$K_2$ | 0 | 0 | $-(S_T-K_2)$ |
| Total | 0 | $S_T-K_1$ | $K_2-K_1$ |

*   Bear spreads: long put $K_1$ and short put $K_2$ with $K_1 > K_2$.

| | $S_T \le K_2$ | $K_2 < S_T \le K_1$ | $S_T \ge K_1$ |
| :-------- | :----------- | :------------------ | :---------- |
| +Put@$K_1$ | $K_1-S_T$ | $K_1-S_T$ | 0 |
| -Put@$K_2$ | $-(K_2-S_T)$ | 0 | 0 |
| Total | $K_1-K_2$ | $K_1-S_T$ | 0 |

## Option Strategies

*   Butterfly spreads: long call $K_1$, long call $K_3$ and short 2 calls with $K_2$ where $K_1 < K_2 < K_3$

| $K_2 = 0.5(K_1 + K_3)$ | $S_T \le K_1$ | $K_1 < S_T \le K_2$ | $K_2 < S_T \le K_3$ | $S_T \ge K_3$ |
| :---------------------- | :----------- | :------------------ | :------------------ | :---------- |
| +Call@$K_1$ | 0 | $S_T-K_1$ | $S_T-K_1$ | $S_T-K_1$ |
| +Call@$K_3$ | 0 | 0 | 0 | $S_T-K_3$ |
| -2Call@$K_2$ | 0 | 0 | $-2(S_T-K_2)$ | $-2(S_T-K_2)$ |
| Total | 0 | $S_T-K_1$ | $K_3-S_T$ | 0 |

*   Strangles: buy call $K_1$ and buy put $K_2$, where $K_2 \le K_1$ (if $K_1 = K_2$ it is called straddle).

| | $S_T \le K_2$ | $K_2 < S_T \le K_1$ | $S_T \ge K_1$ |
| :-------- | :----------- | :------------------ | :---------- |
| +Call@$K_1$ | 0 | 0 | $S_T-K_1$ |
| +Put@$K_2$ | $K_2-S_T$ | 0 | 0 |
| Total | $K_2-S_T$ | 0 | $S_T-K_1$ |

## Portfolio Insurance

*   Insuring against a loss without relinquishing the upside.
    *   Protective put
    *   Purchasing a bond and a call option

## Put-Call Parity

*   Purchasing the underlying asset and a put provides exactly the same payoff from purchasing a bond and a call. Then, by the Law of One Price they must have the same price.
    $$S + P = PV(K) + C$$
    Put-call parity
    $$C + \frac{K}{(1+r_f)^T} = S_0 + P$$
    Calls are equivalent to long positions in puts, buying the underlying asset and (partially) financing the purchases by borrowing the PV of the strike price of the options.
    $$C = S_0 + P - \frac{K}{(1+r_f)^T}$$
    Puts are equivalent to long positions in calls, shorting the underlying asset and using the proceeds to lend the PV of the strike price of the options.
    $$P = C - S_0 + \frac{K}{(1+r_f)^T}$$

## Put-Call Parity

*   It is possible to buy three-month call options and three-month puts on stock Q. Both options have an exercise price of $60 and both are worth $10. If the interest rate is 5% a year, what is the stock price?
    $$C = S_0 + P - \frac{K}{(1+r_f)^T}$$
    $$C = P, \quad r_f = 5\%, \quad K = 60, \quad T = 0.25$$
    $$S_0 = \frac{K}{(1+r_f)^T} = \frac{60}{(1+0.05)^{0.25}} = \$59.27$$
*   A stock is currently selling for $47 per share. A call option with an exercise price of $50 sells for $3.80 and expires in three months. If the risk-free rate of interest is 2.6 percent per year, compounded continuously, what is the price of a put option with the same exercise price?
    $$C = S_0 + P - Ke^{-rT}$$
    $$3.80 = 47 + P - 50e^{-0.026 \times 0.25}$$
    $$P = \$6.48$$
*   A put option that expires in six months with an exercise price of $75 sells for $4.89. The stock is currently priced at $72, and the risk-free rate is 3.6 percent per year, compounded continuously. What is the price of a call option with the same exercise price?
    $$C = 72 + 4.89 - 75e^{-0.036 \times 0.5} = \$3.23$$

## Factors Affecting Option Prices

*   Strike Price and Stock Price
    *   The value of an otherwise identical call option is higher if the strike price the holder must pay to buy the stock is lower. $\max(S_T – K, 0)$
    *   Puts with a lower strike price are less valuable. $\max(K – S_T, 0)$
*   Arbitrage Bounds on Option Prices
    *   A put option cannot be worth more than its strike price.
    *   A call option cannot be worth more than the stock itself.
    *   An American option cannot be worth less than its European counterpart.
    *   An American option cannot be worth less than its intrinsic value.
        *   The intrinsic value of an option is the value it would have if it expired immediately.
    *   An American option cannot have a negative time value.
        *   The time value of an option is the difference between the current option price and its intrinsic value.

## Factors Affecting Option Prices

*   Option Prices and the Exercise Date
    *   An American option with a later exercise date cannot be worth less than an otherwise identical American option with an earlier exercise date.
    *   A European option with a later exercise date may potentially trade for less than an otherwise identical option with an earlier exercise date.
*   Option Prices and Volatility
    *   The value of an option generally increases with the volatility of the stock.
        *   An increase in volatility increases the likelihood of very high and very low returns for the stock.
        *   The holder of a call option benefits from a higher payoff when the stock goes up and the option is in-the-money, but earns the same (zero) payoff no matter how far the stock drops once the option is out-of-the-money.
        *   Insurance is more valuable when there is higher volatility—hence put options on more volatile stocks are also worth more.

## Exercising Options Early

*   Non-Dividend-Paying Stocks
    $$C = P + S - PV(K) \quad \text{If} \quad PV(K) = K - dis(K)$$
    $$C = \frac{S-K}{\text{Intrinsic Value}} + \frac{dis(K) + P}{\text{Time Value}}$$
    where $dis(K)$ is the amount of the discount from face value to account for interest.
    *   The price of any call option on a non-dividend-paying stock always exceeds its intrinsic value.
    *   It is never optimal to exercise a call option on a non-dividend paying stock early.
    *   Always better off just selling the option.
    *   An American call on a non-dividend-paying stock has the same price as its European counterpart.
    *   Under certain circumstances, exercising an American put option on a non-dividend-paying stock might make sense.
    $$P = \frac{K-S}{\text{Intrinsic Value}} + \frac{C - dis(K)}{\text{Time Value}}$$
    *   The European put may sell for less than its intrinsic value.
    *   American put cannot sell for less than its intrinsic value.
    *   The American option can be worth more than an otherwise identical European option.

## Exercising Options Early

*   Dividend-Paying Stocks
    $$C = P + S - PV(Div) – PV(K) \quad \text{If} \quad PV(K) = K - dis(K)$$
    $$C = \frac{S-K}{\text{Intrinsic Value}} + \frac{dis(K) + P – PV(Div)}{\text{Time Value}}$$
    where $dis(K)$ is the amount of the discount from face value to account for interest.
    *   If $PV(Div)$ is large enough, the time value of a European call option can be negative.
    *   The price of the American option can exceed the price of a European option.
        *   When a company pays a dividend, investors expect the price of the stock to drop to reflect the cash paid out.
        *   This price drop hurts the owner of a call option because the stock price falls.
        *   By exercising early, the owner of the call option can capture the value of the dividend.
    $$P = \frac{K-S}{\text{Intrinsic Value}} + \frac{C – dis(K) + PV(Div)}{\text{Time Value}}$$
    *   Dividends reduce the likelihood of early exercise of a put.
    *   The likelihood of early exercise increases whenever the stock goes ex-dividend.

## Exercising Options Early

*   The stock of Harford Inc. is about to pay a $0.30 dividend. It will pay no more dividends for the next month. Consider call options that expire in one month. If the interest rate is 6% APR (monthly compounding), what is the maximum strike price where it could be possible that early exercise of the call option is optimal?
    $$C = \frac{S-K}{\text{Intrinsic Value}} + \frac{dis(K) + P – PV(Div)}{\text{Time Value}}$$
    $$dis(K) – PV(Div) < dis(K) + P – PV(Div) < 0$$
    $$K – K(1 + 0.005)^{-1} < 0.30 \rightarrow K < 60.30$$
*   Suppose the S&P 500 is at 2700, and it will pay a dividend of $90 at the end of the year. Suppose also that the interest rate is 2%. If a one-year European put option has a negative time value, what is the lowest possible strike price it could have?
    $$P = \frac{K-S}{\text{Intrinsic Value}} + \frac{C – dis(K) + PV(Div)}{\text{Time Value}}$$
    $$PV(Div) – dis(K) < C - dis(K) + PV(Div) < 0$$
    $$\frac{90}{(1.02)} < K – K(1 + 0.02)^{-1} \rightarrow K > 4,500$$

## Options and Corporate Finance

*   Equity as a Call Option
    *   Residual claim
        *   Value of the firm's assets exceeds the required debt payment.
        *   Value of the firm's assets is less than the required debt payment.
*   Debt as an Option Portfolio
    *   The payoff to debt can be viewed as,
        *   The firm's assets, less the equity call option.
        *   A risk-free bond, less a put option on the assets with a strike price equal to the required debt payment.
    Risky debt = Risk-free debt - Put option on firm assets
    Risk-free debt = Risky debt + Put option on firm assets

## Pricing Risky Debt

*   As of September 2012, Google (GOOG) had no debt. Suppose the firm's managers consider recapitalizing the firm by issuing zero-coupon debt with a face value of $163.5 billion due in January of 2014, and using the proceeds to pay a special dividend. Suppose too that Google had 327 million shares outstanding, trading at $700.77 per share, implying a market value of $229.2 billion. The risk-free rate is 0.25%. The current value of a call option with a strike price of $500 is $222.05 per share. Estimate the credit spread Google would have to pay on the debt assuming perfect capital markets.
    *   Assuming perfect capital markets, the total value of Google's equity and debt should remain unchanged after the recapitalization.
    *   The $163.5 billion face value of the debt is equivalent to a claim of $163.5 billion/(327 million shares) = $500 per share on Google's current assets.
    *   Total value of the equity after recap
        *   P(Call option with K=500) * Shares Outstanding
        *   $222.05 * 327 million shares = $72.6 billion
    *   Value of the new debt=Total Value-Equity Value
        *   229.2 - 72.6 = $156.6
    $$PV(Debt) = \frac{FV(Debt)}{(1+r)^t} \rightarrow 156.6 = \frac{163.5}{(1+r)^{16/12}}$$
    $$r = \left(\frac{163.5}{156.6}\right)^{12/16} - 1 = 3.29\%$$
    $$Spread = 3.29\% - 0.25\%$$

## Exercises

*   You own a call option on Intuit stock with a strike price of $40. The option will expire in exactly three months' time.
    *   If the stock is trading at $55 in three months, what will be the payoff of the call?
    *   If the stock is trading at $35 in three months, what will be the payoff of the call?
    *   Payoff diagram?
    $$Payoff = \begin{cases} \max(S_T - K, 0) & \text{if } S_T = 55 \\ \max(S_T - K, 0) & \text{if } S_T = 35 \end{cases}$$
    $$Payoff = \begin{cases} \max(55 - 40, 0) = 15 \\ \max(35 - 40, 0) = 0 \end{cases}$$

## Exercises

*   You wrote a call option on Intuit stock with a strike price of $40. The option will expire in exactly three months' time.
    *   If the stock is trading at $55 in three months, what will be the payoff of the call?
    *   If the stock is trading at $35 in three months, what will be the payoff of the call?
    *   Payoff diagram?
    $$Payoff = \begin{cases} -\max(S_T - K, 0) & \text{if } S_T = 55 \\ -\max(S_T - K, 0) & \text{if } S_T = 35 \end{cases}$$
    $$Payoff = \begin{cases} -\max(55 - 40, 0) = -15 \\ -\max(35 - 40, 0) = 0 \end{cases}$$

## Exercises

*   You own a put option on Ford stock with a strike price of $10. The option will expire in exactly six months' time.
    *   If the stock is trading at $8 in six months, what will be the payoff of the put?
    *   If the stock is trading at $20 in six months, what will be the payoff of the put?
    *   Payoff diagram?
    $$Payoff = \begin{cases} \max(K - S_T, 0) & \text{if } S_T = 8 \\ \max(K - S_T, 0) & \text{if } S_T = 20 \end{cases}$$
    $$Payoff = \begin{cases} \max(10 - 8, 0) = 2 \\ \max(10 - 20, 0) = 0 \end{cases}$$

## Exercises

*   You wrote a put option on Ford stock with a strike price of $10. The option will expire in exactly six months' time.
    *   If the stock is trading at $8 in six months, what will be the payoff of the put?
    *   If the stock is trading at $20 in six months, what will be the payoff of the put?
    *   Payoff diagram?
    $$Payoff = \begin{cases} -\max(K - S_T, 0) & \text{if } S_T = 8 \\ -\max(K - S_T, 0) & \text{if } S_T = 20 \end{cases}$$
    $$Payoff = \begin{cases} -\max(10 - 8, 0) = -2 \\ -\max(10 - 20, 0) = 0 \end{cases}$$

## Exercises

*   What position has more downside exposure: a short position in a call or a short position in a put?
    $$-\max(S_T – K, 0) \quad \text{vs.} \quad -\max(K – S_T, 0)$$

## Exercises

*   Dynamic Energy Systems stock is currently trading for $31 per share. The stock pays no dividends. A one-year European put option on Dynamic with a strike price of $41 is currently trading for $10.24. If the risk-free interest rate is 3% per year, what is the price of a one-year European call option on Dynamic with a strike price of $41?
    $$C = S_0 + P - \frac{K}{(1+r_f)^T} = 31 + 10.24 - \frac{41}{(1 + 0.03)^1} = \$1.4342$$
*   A put option and a call option with an exercise price of $55 expire in two months and sell for $2.65 and $5.32, respectively. If the stock is currently priced at $57.30, what is the annual continuously compounded rate of interest?
    $$C = S_0 + P - Ke^{-rT}$$
    $$5.32 = 57.30 + 2.65 – 55e^{-r \times (\frac{2}{12})}$$
    $$r = 4.05\%$$

## Exercises

*   The current stock price of Intrawest is $20 per share and the one-year risk-free interest rate is 8%. A one-year put on Intrawest with a strike price of $18 sells for $3.33, while the identical call sells for $7.
    *   Is there an arbitrage opportunity?
    *   What must you do to exploit this arbitrage opportunity?
    $$C = S_0 + P - \frac{K}{(1+r_f)^T} = 20 + 3.33 - \frac{18}{(1 + 0.08)^1} = \$6.67 < \$7$$
    *   Calls are equivalent to long positions in puts, buying the underlying asset and (partially) financing the purchases by borrowing the PV of the strike price of the options.
    *   So, sell a call @$7, borrow PV(K=18), buy the stock @$20, buy a put @$3.33

| | Today | @Expiration if $S_T \le K$ | @Expiration if $S_T > K$ |
| :---------------- | :------ | :------------------------- | :------------------------- |
| Sell Call | +7 | 0 | $-(S_T - K)$ |
| Borrow PV(K) | +16.67 | -K | -K |
| Buy Stock @ $20 | -20 | $S_T$ | $S_T$ |
| Buy Put | -3.33 | $(K - S_T)$ | 0 |
| **Overall** | **0.3367** | **0** | **0** |

## Exercises

*   LNUX's stock is currently trading for $4.59. There are puts and calls traded on LNUX. In particular, you know that a call option with a strike of $4.25 which matures one year from today is trading in the market for $0.85. The risk-free rate is 5% (in annual terms).
    *   What should the put trade at if there are no arbitrage opportunities?
    *   If the put was trading at $0.20, how could you construct an arbitrage strategy? Assume you can take long or short positions at the given prices, as well as lend or borrow at the risk-free rate.
    *   If the put was trading at $0.40, how could you construct an arbitrage strategy?
    $$P = C - S_0 + \frac{K}{(1+r_f)^T} = 0.85 – 4.59 + \frac{4.25}{(1 + 0.05)^1} = \$0.3076$$
    If the put was trading at $0.20, then it is cheap.

| | Today | @Expiration if $S_T \le K$ | @Expiration if $S_T > K$ |
| :---------------- | :------ | :------------------------- | :------------------------- |
| Buy Put | -0.20 | $(K - S_T)$ | 0 |
| Borrow PV(K) | +4.0476 | -K | -K |
| Buy Stock @ $4.59 | -4.59 | $S_T$ | $S_T$ |
| Sell Call | +0.85 | 0 | $-(S_T - K)$ |
| **Overall** | **0.1076** | **0** | **0** |

## Exercises

*   LNUX's stock is currently trading for $4.59. There are puts and calls traded on LNUX. In particular, you know that a call option with a strike of $4.25 which matures one year from today is trading in the market for $0.85. The risk-free rate is 5% (in annual terms).
    *   What should the put trade at if there are no arbitrage opportunities?
    *   If the put was trading at $0.20, how could you construct an arbitrage strategy? Assume you can take long or short positions at the given prices, as well as lend or borrow at the risk-free rate.
    *   If the put was trading at $0.40, how could you construct an arbitrage strategy?
    $$P = C - S_0 + \frac{K}{(1+r_f)^T} = 0.85 – 4.59 + \frac{4.25}{(1 + 0.05)^1} = \$0.3076$$
    If the put was trading at $0.40, then it is expensive.

| | Today | @Expiration if $S_T \le K$ | @Expiration if $S_T > K$ |
| :---------------- | :------ | :------------------------- | :------------------------- |
| Sell Put | +0.40 | $-(K - S_T)$ | 0 |
| Sell Stock @ $4.59 | +4.59 | $-S_T$ | $-S_T$ |
| Lend PV(K) | -4.0476 | +K | +K |
| Buy Call | -0.85 | 0 | $(S_T - K)$ |
| **Overall** | **0.0924** | **0** | **0** |

## Exercises

*   AGE Corp shares are currently trading at $83. Risk-free rate is 6% per year, compounded continuously. Consider options on AGE Corp stock with an exercise price of $80 and 6 month to maturity. Current price of a put is $8.13.
    *   What is the intrinsic value of the call option? Of the put option?
    *   What is the time value of the call option? Of the put option?
    $$C = \frac{S-K}{\text{Intrinsic Value}} + \frac{dis(K) + P}{\text{Time Value}}$$
    $$P = \frac{K-S}{\text{Intrinsic Value}} + \frac{C - dis(K)}{\text{Time Value}}$$
    $$C_{Intrinsic} = \max[S – K, 0] = 3$$
    $$P_{Intrinsic} = \max[K – S, 0] = 0$$
    $$C = S_0 + P - Ke^{-rT} = 83 + 8.13 – 80 \times e^{-0.06 \times 0.5} = \$13.49$$
    $$C_{Time} = dis(K) + P = K – Ke^{-rT} + P = \$10.49$$
    $$P_{Time} = P - P_{Intrinsic} = \$8.13$$
*   Suppose the S&P 500 is at 889, and a one-year European call option with a strike price of $429 has a negative time value. If the interest rate is 6%, what can you conclude about the dividend yield of the S&P 500? (Assume all dividends are paid at the end of the year.)
    $$C = \frac{S-K}{\text{Intrinsic Value}} + \frac{dis(K) + P – PV(Div)}{\text{Time Value}}$$
    $$dis(K) – PV(Div) < dis(K) + P – PV(Div) < 0$$
    $$429 – 429(1.06)^{-1} < PV(Div) \rightarrow PV(Div) > \$24.28$$
    $$Dividend \ Yield > (24.28 \times 1.06)/889 = 2.90\%$$

## Exercises

*   Use the option data from July 13, 2009, in the following table to determine the rate Google would have paid if it had issued $128 billion in zero-coupon debt due in January 2011. Suppose Google currently had 320 million shares outstanding, implying a market value of $135.1 billion. The risk-free rate is 1.00%. (Assume perfect capital markets.)

| GOOG | 422.27 +7.87 | Vol 2177516 | |
| :-------------- | :---------- | :---------- | :-------- |
| Jul 13 2009 @ 13:10 ET | | | |
| Calls | Bid | Ask | Open Int |
| 11 Jan 150.0 (OZF AJ) | 273.60 | 276.90 | 100 |
| 11 Jan 160.0 (OZF AL) | 264.50 | 267.20 | 82 |
| 11 Jan 200.0 (OZF AA) | 228.90 | 231.20 | 172 |
| 11 Jan 250.0 (OZF AU) | 186.50 | 188.80 | 103 |
| 11 Jan 280.0 (OZF AX) | 162.80 | 165.00 | 98 |
| 11 Jan 300.0 (OZF AT) | 148.20 | 150.10 | 408 |
| 11 Jan 320.0 (OZF AD) | 133.90 | 135.90 | 63 |
| 11 Jan 340.0 (OZF AI) | 120.50 | 122.60 | 99 |
| 11 Jan 350.0 (OZF AK) | 114.10 | 116.10 | 269 |
| 11 Jan 360.0 (OZF AM) | 107.90 | 110.00 | 66 |
| 11 Jan 380.0 (OZF AZ) | 95.80 | 98.00 | 88 |
| 11 Jan 400.0 (OZF AU) | 85.10 | 87.00 | 2577 |
| 11 Jan 420.0 (OUP AG) | 74.60 | 76.90 | 66 |
| 11 Jan 450.0 (OUP AV) | 61.80 | 63.30 | 379 |

    *   Assuming perfect capital markets, the total value of Google's equity and debt should remain unchanged after the recapitalization.
    *   The $128.0 billion face value of the debt is equivalent to a claim of $128.0 billion/(320 million shares) = $400 per share on Google's current assets.
    *   Total value of the equity after recap
        *   P(Call option with K=400) * Shares Outstanding
        *   $86.05 * 320 million shares = $27.54 billion
    *   Value of the new debt=Total Value-Equity Value
        *   135.1 - 27.54 = $107.56
    $$PV(Debt) = \frac{FV(Debt)}{(1+r)^t} \rightarrow 107.56 = \frac{128.0}{(1+r)^{18/12}}$$
    $$r = \left(\frac{128}{107.56}\right)^{12/18} - 1 = 12.3\%$$
    $$Spread = 12.3\% – 1.00\%$$

## What is next?

*   Derivatives III
    *   Binomial Option Pricing Model
    *   Black-Scholes Option Pricing Model
    *   Reading(s):
        *   BKM: Ch. 21
    *   Suggested Problems
        *   Chapter 20: 6, 7, 8, 10, 20, 30
```