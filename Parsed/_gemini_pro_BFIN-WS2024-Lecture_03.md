```markdown
# Investments: Finance 2 - BFIN (Lecture 3)

## Outline
*   Fixed-Income Securities II
    *   Managing Bond Portfolios
        *   Interest rate risk
            *   Interest rate sensitivity of bond prices
            *   Duration and its determinants
        *   Convexity
        *   Passive and active management strategies

## Interest Rate Risk
*   Bond prices and yields are inversely related
*   An increase in a bond's yield to maturity causes smaller price change than a decrease of equal magnitude
*   Long-term bonds tend to be more price sensitive than short-term bonds

YTM and Price of a Bond @C=10%

| Bond | Coupon | Maturity | Initial YTM |
|---|---|---|---|
| A | 12% | 5 years | 10% |
| B | 12% | 30 years | 10% |
| C | 3% | 30 years | 10% |
| D | 3% | 30 years | 6% |

### Prices of 8% Coupon Bond (Coupons Paid Semiannually)

| Yield to Maturity (APR) | $T = 1$ Year | $T = 10$ Years | $T = 20$ Years |
|---|---|---|---|
| 8% | 1,000.00 | 1,000.00 | 1,000.00 |
| 9% | 990.64 | 934.96 | 907.99 |
| Fall in price (%)* | 0.94% | 6.50% | 9.20% |
*Equals value of bond at a 9% yield to maturity divided by value of bond at (the original) 8% yield, minus 1.

### Prices of Zero-Coupon Bond(Semiannual Compounding)

| Yield to Maturity (APR) | $T = 1$ Year | $T = 10$ Years | $T = 20$ Years |
|---|---|---|---|
| 8% | 924.56 | 456.39 | 208.29 |
| 9% | 915.73 | 414.64 | 171.93 |
| Fall in price (%)* | 0.96% | 9.15% | 17.46% |
*Equals value of bond at a 9% yield to maturity divided by value of bond at (the original) 8% yield, minus 1.

### Duration
*   A measure of the effective maturity of a bond
*   The weighted average of the times until each payment is received
*   The weights are proportional to the present value of the payment
    *   Duration = Maturity for zero coupon bonds
    *   Duration < Maturity for coupon bonds

$$D = \sum_{t=1}^{T} t \times w_t$$

$$w_t = \frac{CF_t/((1+y)^t)}{P}$$

$CF_t$: Cash flow at time t
$P$: Price of the bond
$y$: Yield to maturity

*   Duration is a key concept in fixed-income portfolio management.
    *   A simple summary statistic of the effective average maturity of the portfolio.
    *   An essential tool in immunizing portfolios from interest rate risk.
    *   A measure of the interest rate sensitivity of a portfolio.

### Duration-Price Relationship
*   Price change is proportional to duration.
*   The percentage change in bond price is the product of modified duration and the change in the bond's yield to maturity.

$$\frac{\Delta P}{P} = -D \times \frac{\Delta y}{1+y}$$

$$\frac{\Delta P}{P} = -D_M \Delta y$$

$$D_M = \frac{D}{1 + y}$$

$D_M$: Modified duration

12% annual coupon, 5y bond

| t | PV(CF) | $w_t$ | $t*w_t$ |
|---|---|---|---|
| 0.0 | | | |
| 1.0 | 1,071.43 | 0.11 | 0.1071 |
| 2.0 | 956.63 | 0.10 | 0.1913 |
| 3.0 | 854.14 | 0.09 | 0.2562 |
| 4.0 | 762.62 | 0.08 | 0.3050 |
| 5.0 | 6,355.18 | 0.64 | 3.1776 |
| Price | 10,000.00 | 1.00 | |
| | | D | 4.0373 |
| | | $D_M$ | 3.6048 |

| t | PV(CF) | $w_t$ | $t*w_t$ |
|---|---|---|---|
| 0.0 | | | |
| 0.5 | 566.04 | 0.06 | 0.0283 |
| 1.0 | 534.00 | 0.05 | 0.0534 |
| 1.5 | 503.77 | 0.05 | 0.0756 |
| 2.0 | 475.26 | 0.05 | 0.0951 |
| 2.5 | 448.35 | 0.04 | 0.1121 |
| 3.0 | 422.98 | 0.04 | 0.1269 |
| 3.5 | 399.03 | 0.04 | 0.1397 |
| 4.0 | 376.45 | 0.04 | 0.1506 |
| 4.5 | 355.14 | 0.04 | 0.1598 |
| 5.0 | 5,918.98 | 0.59 | 2.9595 |
| Price | 10,000.00 | 1.00 | |
| | | D | 3.9008 |
| | | $D_M$ | 3.6800 |

*   Rule 1: The duration of a zero-coupon bond equals its time to maturity.
*   Rule 2: Holding maturity constant, a bond's duration is higher when the coupon rate is lower.
*   Rule 3: Holding the coupon rate constant, a bond's duration generally increases with its time to maturity.
*   Rule 4: Holding other factors constant, the duration of a coupon bond is higher when the bond's yield to maturity is lower.
*   Rule 5: The duration of a level perpetuity is equal to: $\frac{1+y}{y}$

Coupon Rates (per Year)

| Maturity (years) | 2% | 4% | 6% | 8% | 10% |
|---|---|---|---|---|---|
| 1 | 0.995 | 0.990 | 0.985 | 0.981 | 0.976 |
| 5 | 4.742 | 4.533 | 4.361 | 4.218 | 4.095 |
| 10 | 8.762 | 7.986 | 7.454 | 7.067 | 6.772 |
| 20 | 14.026 | 11.966 | 10.922 | 10.292 | 9.870 |
| Infinite (perpetuity) | 13.000 | 13.000 | 13.000 | 13.000 | 13.000 |
Bond durations (YTM = 8% BEY; semiannual coupons)

Δy vs. ΔP

12%, 5Y Bond

| y' | $\Delta y$ | P' | $\Delta$ Price | D | $D_M$ |
|---|---|---|---|---|---|
| 10.00% | -200 | 10,772.17 | 7.72% | 3.95 | 3.76 |
| 10.50% | -150 | 10,572.16 | 5.72% | 3.93 | 3.74 |
| 11.00% | -100 | 10,376.88 | 3.77% | 3.92 | 3.72 |
| 11.50% | -50 | 10,186.20 | 1.86% | 3.91 | 3.70 |
| 12.00% | 0 | 10,000.00 | 0.00% | 3.90 | 3.68 |
| 12.50% | 50 | 9,818.16 | -1.82% | 3.89 | 3.66 |
| 13.00% | 100 | 9,640.56 | -3.59% | 3.88 | 3.64 |
| 13.50% | 150 | 9,467.09 | -5.33% | 3.87 | 3.62 |
| 14.00% | 200 | 9,297.64 | -7.02% | 3.85 | 3.60 |

12%, 10Y Bond

| P' | $\Delta$ Price | D | $D_M$ |
|---|---|---|---|
| 11,246.22 | 12.46% | 6.31 | 6.01 |
| 10,915.17 | 9.15% | 6.25 | 5.94 |
| 10,597.52 | 5.98% | 6.20 | 5.87 |
| 10,292.66 | 2.93% | 6.14 | 5.80 |
| 10,000.00 | 0.00% | 6.08 | 5.73 |
| 9,718.98 | -2.81% | 6.02 | 5.67 |
| 9,449.07 | -5.51% | 5.96 | 5.60 |
| 9,189.77 | -8.10% | 5.90 | 5.53 |
| 8,940.60 | -10.59% | 5.85 | 5.46 |

8%, 10Y Bond

| P' | $\Delta$ Price | D | $D_M$ |
|---|---|---|---|
| 8,753.78 | 13.60% | 6.84 | 6.51 |
| 8,474.72 | 9.98% | 6.78 | 6.44 |
| 8,207.44 | 6.51% | 6.72 | 6.37 |
| 7,951.38 | 3.18% | 6.67 | 6.30 |
| 7,706.02 | 0.00% | 6.61 | 6.23 |
| 7,470.84 | -3.05% | 6.55 | 6.16 |
| 7,245.37 | -5.98% | 6.49 | 6.09 |
| 7,029.17 | -8.78% | 6.43 | 6.02 |
| 6,821.80 | -11.47% | 6.37 | 5.95 |

*   Modified duration is proportional to the derivative of the bond's price with respect to changes in the bond's yield.
*   For small changes in yield,

$$D_M = -\frac{1}{P} \frac{dP}{dy}$$

$$P = \sum_{t=1}^{T} \frac{CF_t}{(1+y)^t}$$

Money Duration $= D_M \times (-P) = -\frac{dP}{dy}$

*   Money (dollar) duration is the negative of the first derivative of a bond's price with respect to its yield.
*   The money duration of a portfolio is just the sum of the dollar duration of the various instruments in the portfolio.
*   DV01 is the dollar value of a basis point.

A bond with a par value of €10,000, a maturity of 4 years, semiannual coupon payments, has a price of €9,326.72 and a yield to maturity of 8%.
What is the annual coupon rate?
What is the duration of the bond at the current price?
What is the modified duration?
Estimate the price of the bond given a 50 basis points decline in the YTM.
What is the actual price of the bond when the YTM declines to 7.5%?

$$\text{€}9,326.72 = \sum_{t=1}^{8} \frac{C_t}{(1+4\%)^t} + \frac{\text{Par Value}}{(1+4\%)^8}$$

$C = \text{€}300$
Annual coupon rate $= \frac{\text{€}300 \times 2}{\text{€}10,000} = 6\%$

$$D_M = \frac{D}{(1 + y/2)} = \frac{3.60}{(1 + 0.04)} = 3.4615$$

$$\frac{\Delta P}{P} = -D_M \Delta y = -3.4615 \times -0.5\% = 1.73\%$$

$$P' = \sum_{t=1}^{8} \frac{300}{(1+3.75\%)^t} + \frac{10,000}{(1 + 3.75\%)^8} = \text{€}9,489.79$$

$$\frac{\Delta P}{P} = \frac{9,489.79}{9,326.72} - 1 = 1.75\%$$

| t | PV(CF)@8% | $w_t$@8% | $t*w_t$@8% | PV(CF)@7.5% | $w_t$@7.5% | $t*w_t$@7.5% |
|---|---|---|---|---|---|---|
| 0.0 | | | | | | |
| 0.5 | 288.46 | 0.03 | 0.0155 | 289.16 | 0.03 | 0.0152 |
| 1.0 | 277.37 | 0.03 | 0.0297 | 278.71 | 0.03 | 0.0294 |
| 1.5 | 266.70 | 0.03 | 0.0429 | 268.63 | 0.03 | 0.0425 |
| 2.0 | 256.44 | 0.03 | 0.0550 | 258.92 | 0.03 | 0.0546 |
| 2.5 | 246.58 | 0.03 | 0.0661 | 249.56 | 0.03 | 0.0657 |
| 3.0 | 237.09 | 0.03 | 0.0763 | 240.54 | 0.03 | 0.0760 |
| 3.5 | 227.98 | 0.02 | 0.0856 | 231.85 | 0.02 | 0.0855 |
| 4.0 | 7,526.11 | 0.81 | 3.2278 | 7,672.42 | 0.81 | 3.2340 |
| Totals: | 9,326.73 | 1.00 | 3.60 | 9,489.79 | 1.00 | 3.60 |

A bond with a par value of €10,000, a maturity of 7 years, coupon payments twice a year, an annual coupon of 10%, and a yield to maturity of 8%.
What is the current price of the bond?
What is the duration of the bond at the current price?
What is the modified duration?
Estimate the bond price given a 50 basis points increase in the YTM.
What is the actual price of the bond when the YTM increases to 8.5%?

$$P_0 = \sum_{t=1}^{14} \frac{500}{(1+4\%)^t} + \frac{10,000}{(1 + 4\%)^{14}} = \text{€}11,056.30$$

$$D_M = \frac{D}{(1 + y/2)} = \frac{5.30}{(1 + 0.04)} = 5.10$$

$$\frac{\Delta P}{P} = -D_M \Delta y = -5.10 \times 0.5\% = -2.55\%$$

$$P' = \sum_{t=1}^{14} \frac{500}{(1+4.25\%)^t} + \frac{10,000}{(1 + 4.25\%)^{14}} = \text{€}10,779.30$$

$$\frac{\Delta P}{P} = \frac{10,779.30}{11,056.30} - 1 = -2.51\%$$

| t | PV(CF)@8% | $w_t$@8% | $t*w_t$@8% | PV(CF)@8.5% | $w_t$@8.5% | $t*w_t$@8.5% |
|---|---|---|---|---|---|---|
| 0.0 | | | | | | |
| 0.5 | 480.77 | 0.04 | 0.0217 | 479.62 | 0.04 | 0.0222 |
| 1.0 | 462.28 | 0.04 | 0.0418 | 460.06 | 0.04 | 0.0427 |
| 1.5 | 444.50 | 0.04 | 0.0603 | 441.31 | 0.04 | 0.0614 |
| 2.0 | 427.40 | 0.04 | 0.0773 | 423.32 | 0.04 | 0.0785 |
| 2.5 | 410.96 | 0.04 | 0.0929 | 406.06 | 0.04 | 0.0942 |
| 3.0 | 395.16 | 0.04 | 0.1072 | 389.51 | 0.04 | 0.1084 |
| 3.5 | 379.96 | 0.03 | 0.1203 | 373.63 | 0.03 | 0.1213 |
| 4.0 | 365.35 | 0.03 | 0.1322 | 358.39 | 0.03 | 0.1330 |
| 4.5 | 351.29 | 0.03 | 0.1430 | 343.78 | 0.03 | 0.1435 |
| 5.0 | 337.78 | 0.03 | 0.1528 | 329.77 | 0.03 | 0.1530 |
| 5.5 | 324.79 | 0.03 | 0.1616 | 316.32 | 0.03 | 0.1614 |
| 6.0 | 312.30 | 0.03 | 0.1695 | 303.43 | 0.03 | 0.1689 |
| 6.5 | 300.29 | 0.03 | 0.1765 | 291.06 | 0.03 | 0.1755 |
| 7.0 | 6,063.49 | 0.55 | 3.8389 | 5,863.06 | 0.54 | 3.8074 |
| Totals: | 11,056.31 | 1.00 | 5.30 | 10,779.32 | 1.00 | 5.27 |

### Convexity
*   Duration rule for the impact of interest rates on bond prices is only an approximation.
*   A good approximation for small changes in bond yield, but it is less accurate for larger changes.
*   Duration approximation always understates the value of the bond;
    *   Underestimates the increase in bond price when the yield falls,
    *   Overestimates the decline in price when the yield rises.
*   The curvature of the price-yield curve is called the convexity of the bond.
    *   Convexity is measured as the rate of change of the slope of the price-yield curve, expressed as a fraction of the bond price.

$$\text{Convexity} = \frac{1}{P \times (1 + y)^2} \sum_{t=1}^{T} \left[ \frac{CF_t}{(1 + y)^t} (t^2 + t) \right]$$

$$\frac{\Delta P}{P} = -D_M \Delta y + \frac{1}{2} [\text{Convexity} \times (\Delta y)^2]$$

A bond with a par value of €10,000, a maturity of 8 years, annual coupon payments, an annual coupon rate of 6%, and a yield to maturity of 8%.
Duration of the bond is 6.48. What is the modified duration?
Estimate the bond price given a 50 basis points decline in the YTM.
What is the actual price of the bond when the YTM declines to 7.5%?
What is the convexity of the bond at the current price?

$$P = \sum_{t=1}^{8} \frac{600}{(1+8.0\%)^t} + \frac{10,000}{(1 + 8.0\%)^8} = \text{€}8,850.67$$

$$D_M = \frac{D}{(1 + y)} = \frac{6.48}{(1 + 0.08/1)} = 6.00$$

$$\text{Convexity} = \frac{1}{P \times (1 + y)^2} \sum_{t=1}^{T} \left[ \frac{CF_t}{(1 + y)^t} (t^2 + t) \right]$$

$$\frac{\Delta P}{P} = -D_M \Delta y = -6.00 \times -0.5\% = 3.00\%$$

$$P' = \sum_{t=1}^{8} \frac{600}{(1+7.5\%)^t} + \frac{10,000}{(1 + 7.5\%)^8} = \text{€}9,121.40$$

$$\frac{\Delta P}{P} = \frac{9,121.40}{8,850.67} - 1 = 3.06\%$$

| t | PV(CF@8.0%) | $w_t$ | $t*w_t$ | Convexity | PV(CF@7.5%) |
|---|---|---|---|---|---|
| 0.0 | | | | | |
| 1.0 | 555.56 | 0.06 | 0.0628 | 0.11 | 558.14 |
| 2.0 | 514.40 | 0.06 | 0.1162 | 0.30 | 519.20 |
| 3.0 | 476.30 | 0.05 | 0.1614 | 0.55 | 482.98 |
| 4.0 | 441.02 | 0.05 | 0.1993 | 0.85 | 449.28 |
| 5.0 | 408.35 | 0.05 | 0.2307 | 1.19 | 417.94 |
| 6.0 | 378.10 | 0.04 | 0.2563 | 1.54 | 388.78 |
| 7.0 | 350.09 | 0.04 | 0.2769 | 1.90 | 361.65 |
| 8.0 | 5,726.85 | 0.65 | 5.1764 | 39.94 | 5,943.44 |
| Totals: | 8,850.67 | 1.00 | 6.48 | 46.38 | 9,121.40 |
| | | $D_M$ | 6.00 | | |

| | Initial Price | Duration Estimate | Convexity Adjustment |
|---|---|---|---|
| Value | 8,850.67 | 9,116.20 | 9,121.33 |
| Percentage | | 3.00% | 0.06% |

A bond with a par value of €10,000, a maturity of 8 years, semiannual coupon payments, an annual coupon rate of 6%, and a yield to maturity of 8%.
Estimate the bond price given a 50 basis points decline in the YTM.
What is the actual price of the bond when the YTM declines to 7.5%?

$$P = \sum_{t=1}^{16} \frac{300}{(1 + 4.0\%)^t} + \frac{10,000}{(1 + 4.0\%)^{16}} = \text{€}8,834.77$$

$$P' = \sum_{t=1}^{16} \frac{300}{(1+3.75\%)^t} + \frac{10,000}{(1 + 3.75\%)^{16}} = \text{€}9,109.74$$

$$\frac{\Delta P}{P} = \frac{9,109.74}{8,834.77} - 1 = 3.112\%$$

$$D_M = \frac{D}{(1 + y/2)} = \frac{6.35}{(1 + 0.08/2)} = 6.11$$

$$\frac{\Delta P}{P} = -D_M \Delta y = -6.11 \times -0.5\% = 3.055\%$$

$$\frac{\Delta P}{P} = -D_M \Delta y + \frac{1}{2} [\text{Convexity} \times (\Delta y)^2] = 3.055\% + \frac{1}{2} [45.98 \times (0.005)^2]$$
$$= 3.055\% + 0.575\% = 3.112\%$$

Par Value: 10,000.00
C (Annual): 6.00%
Frequency: 2
YTM_0: 8.00%
YTM_1: 7.50%

| t | PV(CF@8.0%) | $w_t$ | $t*w_t$ | Convexity | PV(CF@7.5%) |
|---|---|---|---|---|---|
| 0.0 | | | | | |
| 1.0 | 288.46 | 0.03 | 0.0327 | 0.03 | 289.16 |
| 2.0 | 277.37 | 0.03 | 0.0628 | 0.09 | 278.71 |
| 3.0 | 266.70 | 0.03 | 0.0906 | 0.17 | 268.63 |
| 4.0 | 256.44 | 0.03 | 0.1161 | 0.27 | 258.92 |
| 5.0 | 246.58 | 0.03 | 0.1395 | 0.39 | 249.56 |
| 6.0 | 237.09 | 0.03 | 0.1610 | 0.52 | 240.54 |
| 7.0 | 227.98 | 0.03 | 0.1806 | 0.67 | 231.85 |
| 8.0 | 219.21 | 0.02 | 0.1985 | 0.83 | 223.47 |
| 9.0 | 210.78 | 0.02 | 0.2147 | 0.99 | 215.39 |
| 10.0 | 202.67 | 0.02 | 0.2294 | 1.17 | 207.61 |
| 11.0 | 194.87 | 0.02 | 0.2426 | 1.35 | 200.10 |
| 12.0 | 187.38 | 0.02 | 0.2545 | 1.53 | 192.87 |
| 13.0 | 180.17 | 0.02 | 0.2651 | 1.72 | 185.90 |
| 14.0 | 173.24 | 0.02 | 0.2745 | 1.90 | 179.18 |
| 15.0 | 166.58 | 0.02 | 0.2828 | 2.09 | 172.70 |
| 16.0 | 5,499.25 | 0.62 | 9.9593 | 78.27 | 5,715.15 |
| Totals: | 8,834.77 | 1.00 | 6.35 | 45.98 | 9,109.74 |
| | | $D_M$ | 6.11 | | |

| | Initial Price | Duration Estimate | Convexity Adjustment |
|---|---|---|---|
| Value | 8,834.77 | 9,104.59 | 9,109.67 |
| Percentage | | 3.05% | 0.06% |

$$\text{Bond Convexity Approximation} = \frac{P_{up} + P_{Down} - 2 \times P}{P \times (\Delta y)^2}$$

A bond with a par value of €10,000, a maturity of 8 years, semiannual coupon payments, an annual coupon rate of 6%, and a yield to maturity of 8%.
Estimate current bond price and the bond prices given a 50 basis points decline and increase in the YTM.
Calculate the approximate convexity of the bond.

$$P = \sum_{t=1}^{16} \frac{300}{(1+4.0\%)^t} + \frac{10,000}{(1 + 4.0\%)^{16}} = \text{€}8,834.77$$

$$P_{up} = \sum_{t=1}^{16} \frac{300}{(1+3.75\%)^t} + \frac{10,000}{(1 + 3.75\%)^{16}} = \text{€}9,109.74$$

$$P_{Down} = \sum_{t=1}^{16} \frac{300}{(1 + 4.25\%)^t} + \frac{10,000}{(1 + 4.25\%)^{16}} = \text{€}8,569.96$$

$$\text{Bond Convexity Approximation} = \frac{9,109.74 + 8,569.96 - 2 \times 8,834.77}{8,834.77 \times (0.005)^2} = \frac{9,109.74 + 8,569.96 - 2 \times 8,834.77}{0.220869} = 46.00$$

*   Higher Convexity → Bigger price increases when yields fall than the price declines when yields rise.
*   The more volatile interest rates, the more attractive this asymmetry.
*   Bonds with greater convexity → higher prices and/or lower yields, all else equal.

### Price-Yield Curve for a Callable Bond
*   As rates fall, there is a ceiling on the bond's market price, which cannot rise above the call price.
*   Negative convexity

## Passive Management
*   Two passive bond portfolio strategies:
    *   Indexing
        *   Attempts to replicate the performance of a given bond index.
    *   Immunization
        *   Used widely by financial institutions such as insurance companies and pension funds to shield overall financial status from exposure to interest rate fluctuations.
*   Both see market prices as being correct
*   Differ greatly in terms of risk
    *   A bond-index portfolio will have the same risk-reward profile as the bond market index to which it is tied.
    *   Immunization strategies seek to establish a virtually zero-risk profile
        *   Interest rate movements have no impact on the value of the portfolio.

### Passive Management: Indexing
#### Bond Index Funds
*   Contains Thousands of Issues, many of which are infrequently traded
*   Turnover more than stock indexes as the bonds mature
*   They only hold a representative sample of the bonds in the actual index
*   The idea is to create a portfolio that mirrors the composition of an index that measures the broad market.
    *   Broad market indexes
        *   Government, Agencies, Supras
        *   Corporate,
        *   Mortgage-backed securities
        *   Yankee bonds
*   Challenges in constructing an indexed bond portfolio
    *   Indexes include thousands of securities
    *   Many bonds are very thinly traded
    *   Rebalancing problems
        *   Bonds are continually dropped from the index as they approach maturity.
        *   New bonds are added to the index as they are issued.
    *   Bonds generate considerable interest income that must be reinvested.

### Passive Management: Immunization
*   Control interest rate risk
*   Widely used by pension funds, insurance companies, and banks
*   A natural mismatch between asset and liability maturity structures.
    *   Bank liabilities are primarily the deposits owed to customers, most of which are short-term and, consequently, have low duration.
    *   Bank assets by contrast are composed largely of outstanding commercial and consumer loans or mortgages, which have longer duration.
    *   What happens when interest rates rise unexpectedly?
    *   What about the risks pension funds are exposed to?
*   The interest rate exposure of assets and liabilities is matched in the portfolio.
    *   Match the duration of the assets and liabilities.
    *   Price risk and reinvestment rate risk exactly cancel out.
        *   When the portfolio duration equals the investor's horizon date, the accumulated value of the investment fund at the horizon date will be unaffected by interest rate fluctuations.
    *   Value of assets match liabilities whether rates rise/fall.
    *   Duration-matched assets and liabilities let the asset portfolio meet the firm's obligations despite interest rate movements.

*   Duration matching balances the difference between the accumulated value of the coupon payments (reinvestment rate risk) and the sale value of the bond (price risk).
    *   When interest rates fall, the coupons grow less than in the base case, but the higher value of the bond offsets this.
    *   When interest rates rise, the value of the bond falls, but the coupons more than make up for this loss because they are reinvested at the higher rate.

*   Coupon paying bond and single-payment obligation.
    *   For small changes in interest rates, the change in value of both the asset and the obligation is equal, so the obligation remains fully funded.
    *   For greater changes in the interest rate, the present value curves diverge.
    *   Convexity
    *   Rebalancing
        *   Interest rate changes cause mismatch.
        *   Asset durations will change with time.
        *   Without rebalancing, durations will become unmatched.

### Passive Management: Cash Flow Matching and Dedication
*   Cash Flow Matching
    *   Buy a zero-coupon bond with a face value equal to the projected cash outlay.
    *   The cash flow from the bond and the obligation exactly offset each other, no interest rate risk.
*   Dedication strategy
    *   Cash flow matching on a multiperiod basis.
    *   Either zero-coupon or coupon bonds with total cash flows in each period that match a series of obligations.
    *   There is no need for rebalancing once the cash flows are matched.
*   Some Issues
    *   Cash flow matching imposes constraints on bond selection.
    *   Immunization or dedication strategies are appealing to firms/investors that do not wish to bet on general movements in interest rates.
    *   Sometimes, cash flow matching is simply not possible b/c of the availability of assets with required maturities.
*   Other Problems
    *   Duration is calculated using YTM. The implicit assumption is a flat yield curve.
    *   What if the yield curve is not flat as is the case most of the time in the real world?
        *   Discount using the appropriate spot interest rate from the zero-coupon yield curve corresponding to the date of the particular cash flow.
        *   Even with this modification, duration matching will immunize portfolios only for parallel shifts in the yield curve.

## What is next?
*   Portfolio Theory and Practice I
    *   Risk, Return, and the Historical Record
    *   Capital Allocation to Risky Assets
        *   Readings: Ch. 5 & 6
    *   Suggested Problems
        *   Ch. 16: 4, 5, 9, 11, 12, 16, 21, 23
        *   Ch 16 – CFA Problems: 7, 12
```