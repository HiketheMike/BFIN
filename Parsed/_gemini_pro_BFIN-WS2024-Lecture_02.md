```markdown
# Investments

## Outline
*   Fixed-Income Securities I
    *   Bond Prices and Yields
    *   The Term Structure of Interest Rates

## Bond Prices and Yields

### Bond Characteristics
*   A security that is issued in connection with a borrowing arrangement.
    *   Par value or face value
    *   Coupon payments
    *   Coupon rate
    *   Bond indenture
        *   The contract between the issuer and the bondholder

### Government Bonds and Notes
*   Bonds and notes may be purchased directly from the Treasury
    *   Note maturity: 1-10 years
    *   Bond maturity: 10-30 years

U.S. Treasury Quotes:

| MATURITY | COUPON | BID      | ASKED    | ASKED CHANGE | YIELD (%) |
| :------- | :----- | :------- | :------- | :----------- | :-------- |
| Nov 15 20 | 1.750  | 97.8438  | 97.8594  | 0.0156       | 2.860     |
| Nov 15 22 | 1.625  | 95.0547  | 95.0703  | 0.0313       | 2.941     |
| Nov 15 26 | 2.000  | 92.4375  | 92.4531  | 0.1016       | 3.072     |
| Nov 15 26 | 6.500  | 124.4063 | 124.4219 | 0.0781       | 3.037     |
| May 15 30 | 6.250  | 129.8281 | 129.8906 | 0.0547       | 3.134     |
| May 15 37 | 5.000  | 124.5469 | 124.6094 | -0.0547      | 3.223     |
| Feb 15 41 | 4.750  | 122.3438 | 122.4063 | -0.1719      | 3.318     |
| Nov 15 45 | 3.000  | 93.5859  | 93.6172  | -0.0859      | 3.362     |

### Corporate Bonds
*   Callable bonds
    *   Can be repurchased before the maturity date
        *   Call price
        *   Call protection, deferred callable bonds.
*   Puttable Bonds
    *   Give the holder an option to retire or extend the bond
*   Convertible bonds
    *   Can be exchanged for shares of the firm's common stock
    *   Conversion ratio: The number of shares for which each bond may be exchanged.
        *   Market conversion value
        *   Conversion premium
*   Floating-rate bonds
    *   Have adjustable coupon rate
    *   The coupon rate on floaters adjusts to changes in the general level of market interest rates, it does not adjust to changes in financial condition of the issuer.

### Preferred Stock
*   Promises to pay a specified cash flow stream.
    *   Fixed dividend vs. floating-rate
*   Dividends on preferred stock are not considered tax-deductible expenses.
*   Failure to pay the promised dividend does not result in corporate bankruptcy.

**Like Fixed Income**
*   Payments are typically fixed
*   Preferred dividends are paid before common

**Like Equity**
*   Dividends are paid in perpetuity
*   Nonpayment does not mean bankruptcy
*   No tax break

### Other Domestic Issuers
*   Local governments
*   Government agencies

### International Bonds
*   Foreign Bonds
    *   Borrower is from a country other than the one in which the bond is sold.
    *   The bond is denominated in the currency of the country in which it is marketed.
        *   Yankee Bonds
        *   Samurai Bonds
        *   Bulldog Bonds
*   Eurobonds
    *   Denominated in one currency, usually that of the issuer, but sold in other national markets.
        *   Eurodollar
        *   Euroyen
        *   Eurosterling

### Inverse Floaters
*   Similar to the floating-rate bonds.
*   The coupon rate on these bonds falls when the general level of interest rates or reference rate rises.

### Asset-Backed Bonds
*   The income from a specified group of assets is used to service the debt.

### Catastrophe Bonds
*   A way to transfer "catastrophe risk" to the capital markets.
    *   Higher coupon rates
    *   In the event of a catastrophe, the bondholders lose all or part of their investments.
    *   World Bank "pandemic bonds”
        *   Issued in 2018, during COVID-19 $195 million paid to 64 developing countries.

### Indexed Bonds
*   Payments are tied to a reference
    *   Price index
    *   Commodity prices
    *   GDP
*   Treasury Inflation Protected Securities (TIPS)
    *   Consider a newly issued bond with a 3-year maturity, par value of $1,000, and a coupon rate of 4%. Assume that the bond makes annual coupon payments, and inflation turns out to be 2%, 3%, and 1% in the next three years.

| Time | Inflation in Year Just Ended | Par Value | Coupon Payment | + | Principal Repayment | = | Total Payment |
| :--- | :--------------------------- | :-------- | :------------- | :- | :------------------ | :- | :------------ |
| 0    |                              | $1,000.00 |                |    |                     |    |               |
| 1    | 2%                           | 1,020.00  | $40.80         |    | $0                  |    | $40.80        |
| 2    | 3                            | 1,050.60  | 42.02          |    | 0                   |    | 42.02         |
| 3    | 1                            | 1,061.11  | 42.44          |    | 1,061.11            |    | 1,103.55      |

### Bond Pricing
*   The nominal risk-free interest rate equals the sum of
    *   A real risk-free rate of return
    *   A premium above the real rate to compensate for expected inflation.
    *   An additional premium that reflects bond-specific characteristics such as default risk, liquidity, tax attributes, call risk, and so on.

$$ P_B = \sum_{t=1}^{T} \frac{C}{(1+r)^t} + \frac{Par Value}{(1+r)^T} $$

$$ P_B = C * \frac{1}{r} \left[1 - \frac{1}{(1+r)^T}\right] + \frac{Par Value}{(1+r)^T} $$

*   Annual 8% coupon, 30-year maturity bond with par value of $1,000, semiannual coupon payments. Suppose that the interest rate is 10% annually. Then,

$$ P_B = \frac{1,000 \cdot 8\%}{2} \cdot \frac{1}{10\%/2} \left[1 - \frac{1}{(1+10\%/2)^{60}}\right] + \frac{1,000}{(1+10\%/2)^{60}} $$

$P_B = \$810.71$

Bond Price at Given Market Interest Rate

| Time to Maturity | 2%         | 4%         | 6%         | 8%         | 10%        |
| :--------------- | :--------- | :--------- | :--------- | :--------- | :--------- |
| 1 year           | 1,059.11   | 1,038.83   | 1,019.13   | 1,000.00   | 981.41     |
| 10 years         | 1,541.37   | 1,327.03   | 1,148.77   | 1,000.00   | 875.35     |
| 20 years         | 1,985.04   | 1,547.11   | 1,231.15   | 1,000.00   | 828.41     |
| 30 years         | 2,348.65   | 1,695.22   | 1,276.76   | 1,000.00   | 810.71     |

### Accrued Interest and Quoted Bond Prices
*   If a bond is purchased between coupon payments, the buyer must pay the seller for accrued interest.
    *   It is the prorated share of the upcoming semiannual coupon.
    *   The quoted price does not include the interest that accrues between coupon payment dates.

$$ \text{Accrued interest} = \frac{\text{Annual coupon payment}}{2} \times \frac{\text{Days since last coupon payment}}{\text{Days separating coupon payments}} $$

*   30 days have passed since the last coupon payment, and there are 182 days in the semiannual coupon period, face value of $1,000, and the coupon rate is 8%.

$$ \text{Accrued Interest} = \text{Coupon payment} \times \frac{\text{Days since last coupon payment}}{\text{Days separating coupon payments}} $$

$$ \text{Accrued Interest} = \frac{1,000 \cdot 8\%}{2} \cdot \frac{30}{182} = \$6.59 $$

*   Stocks do not trade at flat prices with adjustments for "accrued dividends." Whoever owns the stock when it goes "ex-dividend" receives the entire dividend payment, and the stock price reflects the value of the upcoming dividend.

### Yield to Maturity
*   The interest rate that makes the present value of a bond's payments equal to its price.
*   A measure of the average rate of return that will be earned on a bond if it is bought now and held until maturity.
    *   Assumption: All coupons can be reinvested at YTM

### Current yield
*   The bond's annual coupon payment divided by its price.
*   A 30-year bond selling at $1,276.76, has a face value of $1,000, and pays semiannual coupons of $40.
    *   What is the current yield of the bond?
    *   What average rate of return would be earned by an investor purchasing the bond at this price?

$$ \text{Current Yield} = \frac{\text{Annual Coupon}}{\text{Price}} $$

$$ \text{Current Yield} = \frac{40 \cdot 2}{1,276.76} = 6.27\% $$

$$ P_B = C \cdot \frac{1}{r/2} \left[1 - \frac{1}{(1+r/2)^T}\right] + \frac{\text{Par Value}}{(1+r/2)^T} $$

$1,276.76 = 40 \cdot \frac{1}{r/2} \left[1 - \frac{1}{(1+r/2)^{30 \cdot 2}}\right] + \frac{1,000}{(1+r/2)^{30 \cdot 2}}$

$r/2 = 3\%$
$r = 6\%$

Effective annual yield of the bond = $(1 + r/2)^2 = 6.09\%$

### Yield to Call
*   If the bond is callable, it may be retired prior to the maturity date.
    *   At higher interest rates, the risk of call is negligible.
    *   At lower rates, the values of a callable and straight bond begin to diverge.
    *   The yield to call is calculated just like the yield to maturity
        *   The time until call replaces time until maturity,
        *   The call price replaces par value.
*   A 30-year bond selling at $1,150.00, has a face value of $1,000, and pays semiannual coupons of $40. The bond is callable in 10 years @ $1,100
    *   What is the YTM of the bond?
    *   What is the yield to first call of the bond?

$1,150 = 40 \cdot \frac{1}{r/2} \left[1 - \frac{1}{(1+r/2)^{30 \cdot 2}}\right] + \frac{1,000}{(1+r/2)^{30 \cdot 2}}$
$r = YTM = 6.82\%$

$1,150 = 40 \cdot \frac{1}{r/2} \left[1 - \frac{1}{(1+r/2)^{10 \cdot 2}}\right] + \frac{1,100}{(1+r/2)^{10 \cdot 2}}$
$r = \text{Yield to first call} = 6.64\%$

*   The yield to maturity on two 10-year maturity bonds currently is 7%. Each bond has a call price of $1,100. One bond has a coupon rate of 6%, the other 8%. Assume for simplicity that bonds are called as soon as the present value of their remaining payments exceeds their call price. What will be the capital gain on each bond if the market interest rate suddenly falls to 6%?

$$ P_1 = 30 \cdot \frac{1}{7\%/2} \left[1 - \frac{1}{(1+7\%/2)^{10 \cdot 2}}\right] + \frac{1,000}{(1+7\%/2)^{10 \cdot 2}} $$
$P_1 = \$928.94$

$$ P_2 = 40 \cdot \frac{1}{7\%/2} \left[1 - \frac{1}{(1+7\%/2)^{10 \cdot 2}}\right] + \frac{1,000}{(1+7\%/2)^{10 \cdot 2}} $$
$P_2 = \$1,071.06$

$$ P'_1 = \min \left( 30 \cdot \frac{1}{6\%/2} \left[1 - \frac{1}{(1+6\%/2)^{10 \cdot 2}}\right] + \frac{1,000}{(1+6\%/2)^{10 \cdot 2}} , 1,100 \right) $$
$P'_1 = \min[1,000, 1,100] = \$1,000$

$$ P'_2 = \min \left( 40 \cdot \frac{1}{6\%/2} \left[1 - \frac{1}{(1+6\%/2)^{10 \cdot 2}}\right] + \frac{1,000}{(1+6\%/2)^{10 \cdot 2}} , 1,100 \right) $$
$P'_2 = \min[1,148.77, 1,100] = \$1,100$

Capital Gain(Bond 1) = $1,000 - 928.94 = \$71.06$
Capital Gain(Bond 2) = $1,100 - 1,071.06 = \$28.94$

### Realized Compound Return versus Yield to Maturity
*   Yield to maturity will equal the rate of return realized over the life of the bond if all coupons are reinvested to earn the bond's yield to maturity.

**A: Reinvestment Rate = 10%**
Cash Flow: $100$
Time: $0$, $1$, $2$
Future Value: $1,100 = \$1,100$
$100 \times 1.10 = \$110$
Total: $1,210$

$V^A_0 (1 + r_A)^2 = V^A_2$
$1,000 \cdot (1 + r_A)^2 = 1,210$
$r_A = 10\%$

**B: Reinvestment Rate = 8%**
Cash Flow: $100$
Time: $0$, $1$, $2$
Future Value: $1,100 = \$1,100$
$100 \times 1.08 = \$108$
Total: $1,208$

$V^B_0 (1 + r_B)^2 = V^B_2$
$1,000 \cdot (1 + r_B)^2 = 1,208$
$r_B = 9.91\%$

Price path of two 30-year maturity coupon-paying bonds
The price of a 30-year zero-coupon bond over time

## The Term Structure of Interest Rates

Treasury Yield Curve (January 2006) Flat Yield Curve
Treasury Yield Curve (December 2012) Rising Yield Curve
Treasury Yield Curve (September 11, 2000) Inverted Yield Curve
Treasury Yield Curve (October 4, 1989) Hump-Shaped Yield Curve

*   The pure yield curve refers to the curve for stripped, or zero-coupon, Treasuries.
*   The on-the-run yield curve refers to the plot of yield as a function of maturity for recently issued coupon bonds selling at or near par value.

*   If yields on different-maturity bonds are not all equal, how should we value coupon bonds that make payments at many different times?

| Maturity (years) | Yield to Maturity (%) | Price                     |
| :--------------- | :-------------------- | :------------------------ |
| 1                | 5%                    | $952.38 = \$1,000/1.05$   |
| 2                | 6                     | $890.00 = \$1,000/1.06^2$ |
| 3                | 7                     | $816.30 = \$1,000/1.07^3$ |
| 4                | 8                     | $735.03 = \$1,000/1.08^4$ |

*   What is the price of a 10% coupon bond with a maturity of three years that makes its coupon payments annually.

$$ P_B = \left(100 \cdot \frac{952.38}{1,000}\right) + \left(100 \cdot \frac{890.00}{1,000}\right) + \left(1,100 \cdot \frac{816.30}{1,000}\right) $$
$$ P_B = \frac{100}{(1.05)^1} + \frac{100}{(1.06)^2} + \frac{1,100}{(1.07)^3} $$
$P_B = \$1,082.17$

### The Yield Curve under Certainty
*   Why is the yield on the 2-year zero coupon bond is greater than that on the 1-year zero?

| Maturity (years) | Yield to Maturity (%) | Price                     |
| :--------------- | :-------------------- | :------------------------ |
| 1                | 5%                    | $952.38 = \$1,000/1.05$   |
| 2                | 6                     | $890.00 = \$1,000/1.06^2$ |
| 3                | 7                     | $816.30 = \$1,000/1.07^3$ |
| 4                | 8                     | $735.03 = \$1,000/1.08^4$ |

Buy and hold 2-year zero = Roll over 1-year bonds

$890 \cdot (1+6\%)^2 = 890 \cdot (1 + 5\%)(1 + r_{1,2})$
$r_{1,2} = 7.01\%$

$(1 + 7\%)^3 = (1 + 6\%)^2(1 + r_{2,3})$
$r_{2,3} = 9.03\%$

$(1 + 8\%)^4 = (1 + 7\%)^3(1 + r_{3,4})$
$r_{3,4} = 11.06\%$

Time Line:
Alternative 1: Buy and hold 2-year zero
$0 \rightarrow 1 \rightarrow 2$ (2-Year Investment)
$890 \times 1.06^2 = \$1000$

Alternative 2: Buy a 1-year zero, and reinvest proceeds in another 1-year zero
$0 \rightarrow 1$ (1-Year Investment) $\rightarrow 2$ (1-Year Investment)
$890 \times 1.05 = \$934.50$
$934.50(1+r_2)$

$$ (1 + y_n)^n = (1 + y_{n-1})^{n-1} \cdot (1 + r_n) $$
$$ (1 + r_n) = \frac{(1 + y_n)^n}{(1 + y_{n-1})^{n-1}} $$

Year
$r_1 = 5\%$
$r_2 = 7.01\%$
$r_3 = 9.025\%$
$r_4 = 11.06\%$
Short Rate in Each Year

Current Spot Rates (Yields to Maturity) for Various Maturities
$y_1 = 5\%$ (1-Year Investment)
$y_2 = 6\%$ (2-Year Investment)
$y_3 = 7\%$ (3-Year Investment)
$y_4 = 8\%$ (4-Year Investment)

### Spot rate
*   The yield to maturity on zero-coupon bonds.
*   The rate that prevails today for a time period corresponding to the zero's maturity.

### Short rate
*   The interest rate for a given time interval available at different points in time.

### Forward rate
*   Defined as the “break-even" interest rate that equates the return on an n-period zero-coupon bond to that of an $(n - 1)$-period zero-coupon bond rolled over into a 1-year bond in year n.
*   The interest rate that would need to prevail to make the long- and short-term investments equally attractive, ignoring risk.
    *   When bond prices reflect a risk premium, the forward rate no longer equals the expected short rate.
        *   If most individuals are short-term investors, forward rate must be greater than short rate.
            *   The forward rate will embody a premium compared with the expected future short-interest rate.
        *   If all investors were long-term investors, no one would be willing to hold short-term bonds unless rolling over those bonds offered a reward for bearing interest rate risk.
            *   The forward rate to be less than the expected future spot rate.

### Liquidity
*   Liquidity refers to the ability to sell an asset easily at a predictable price.
*   Long-term bonds have greater price risk, considered less liquid, must offer a premium.

### The liquidity premium
*   The liquidity premium compensates short-term investors for the uncertainty about the price at which they will be able to sell their long-term bonds at the end of the year.

### The Expectations Hypothesis
*   The forward rate equals the market consensus expectation of the future short interest rate,
*   $f_2 = E(r_2)$, and liquidity premiums are zero.
*   Suggests that the yields on long-term bonds depend only on expectations of future short rates.
    *   The forward rates derived from the yield curve can be used to infer market expectations of future short rates.

### Liquidity Preference Theory
*   Short-term investors will be unwilling to hold long-term bonds unless the forward rate exceeds the expected short interest rate.
*   Long-term investors will be unwilling to hold short bonds unless the expected short interest rate exceeds the forward rate.
*   The liquidity preference theory of the term structure argues that short-term investors dominate the market so that the forward rate will generally exceed the expected short rate.

$$ f_n = E(r_n) + \text{Liquidity Premium} $$

## What is next?
### Fixed-Income Securities II
#### Managing Bond Portfolios
*   Readings: Ch. 16

#### Suggested Problems
*   Ch. 14: 6, 10, 14, 21, 23, 29
*   Ch 14 – CFA Problems: 2, 4
*   Ch. 15: 7, 10, 13, 17
*   Ch 15 – CFA Problems: 4, 9
```