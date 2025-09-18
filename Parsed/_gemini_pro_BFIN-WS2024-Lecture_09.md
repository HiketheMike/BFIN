```markdown
# Investments Finance 2 - BFIN

## Outline

*   Derivatives I
    *   Introduction to derivatives
    *   Futures & Forwards
    *   Swaps Contracts

## Introduction to Derivatives

*   A derivative is a financial instrument whose payoffs and values are derived from or depend on an underlying asset.
    *   Futures and Forwards
    *   Options
    *   Swaps
    *   Exotics
*   Derivatives play a key role in transferring risks in the economy.
*   A derivative may be,
    *   A standalone instrument
    *   Embedded in other products

## Introduction to Derivatives

*   The underlying asset
    *   Stocks & Stock indices
    *   Bonds (credit derivatives)
    *   Energy (crude oil, natural gas, power, emissions)
    *   Commodities
        *   Agriculture (grain, pork belly, cattle, sugar, etc).
        *   Metals
    *   Others
        *   Weather (amount of snow, temperature)
        *   Insurance derivatives

## Introduction to Derivatives

*   Types of markets
    *   Exchange traded
        *   Standardized contracts defined by the exchange.
            *   Chicago Board of Trade (CBOT)
            *   Chicago Mercantile Exchange (CME)
            *   Chicago Board Options Exchange (CBOE)
            *   New York Mercantile Exchange (NYMEX)
            *   Intercontinental Exchange (ICE)
    *   Over-the-counter (OTC)
        *   Telephone and computer linked network of dealers/brokers
            *   Financial institutions often act as market makers for the more commonly traded instruments.
        *   More flexibility
        *   Credit/Counterparty risk
        *   Embedded, real options, etc.

## Introduction to Derivatives

*   What are derivatives are used for?
    *   Hedging
        *   Risk management: Cut away unwanted portions of risk exposure and even transform the exposures into quite different forms.
    *   Speculation
        *   No offsetting exposure
    *   To lock in an arbitrage profit
    *   To change the nature of a liability
    *   To change the nature of an investment without incurring the costs of selling one portfolio and buying another.

## Forward Contracts

*   A forward contract is an agreement (contract) to buy or sell an asset at a certain future time for a certain price
    *   An agreement (Forward contract)
    *   To buy / sell an asset (trade Underlying asset)
    *   At future time (Maturity)
    *   For a certain price (Forward price)
*   The buyer and the seller are obligated to perform under the terms of the contract.
*   OTC Transactions

## Forward Contracts

*   Two parties agree to exchange some item in the future at a delivery price specified now.
*   The forward price is defined as the delivery price that makes the current market value of the contract zero.
    *   No money is paid in the present by either party to the other.
*   The face value of the contract is the quantity of the item specified in the contract times the forward price.
*   The party who agrees to buy the specified item is said to take a long position, and the party who agrees to sell the item is said to take a short position.

## Forward Contracts

Arturu Corp will pay £10 million for imports from Britain in 3 months and decides to hedge. What is the appropriate position?

AGE Inc. will receive €10 million for exports to Germany in 6 months and decides to hedge. What is the appropriate position?

*   For $S_T$ = spot price at maturity, and $F$ = Forward price;
    *   The payoff from a long position in a forward contract is: $S_T - F$
    *   The payoff from a short position in a forward contract is: $F – S_T$

## Forward Contracts

*   Since, by definition, the forward price is defined as the delivery price that makes the current market value of the contract zero;
    $$S_0 - PV(F) = 0$$
    $$S_0 = PV(F) = \frac{F}{(1+r)^T}$$
    $$F = S_0(1 + r)^T$$
*   The forward price equals the future value of the spot price compounded at the risk-free interest rate for T years.

Replication of Non-Dividend-Paying Stock Using a Pure Discount Bond and a Stock Forward Contract

| Position                                     | Immediate Cash Flow | Cash Flow 1 Year From Now |
| :------------------------------------------- | :------------------ | :------------------------ |
| Buy a share of stock                         | -$100               | $S_1$                     |
| **Replicating Portfolio (Synthetic Stock):** |                     |                           |
| Go long a forward contract on stock          | 0                   | $S_1 - F$                 |
| Buy a pure discount bond with face value of F | -$F/1.08$            | $F$                       |
| Total replicating portfolio                  | -$F/1.08$            | $S_1$                     |

## Forward Contracts

A trader enters into a one-year short forward contract on 100 million yen. The forward exchange rate is $0.0080 per yen. How much does the trader gain or lose if the exchange rate at the end of the contract is (a) $0.0074 per yen; (b) $0.0091 per yen?

Payoff from a short position: $F – S_T$
$100 \text{ mio} * (0.0080 – 0.0074) = \$60,000$
$100 \text{ mio} * (0.0080 – 0.0091) = -\$110,000$

The price of gold is currently $1,800 per ounce. Forward contracts are available to buy or sell gold at $2,000 per ounce for delivery in one year. An arbitrageur can borrow money at 5% per annum. What should the arbitrageur do? Assume that the cost of storing gold is zero and that gold provides no income.

$S_0' = 2,000(1 + 0.05)^{-1}= 1904.76$

Borrow $\left(\frac{\$2,000}{1.05}\right)$, Buy gold $@1,800$

## Futures Contracts

*   Available on a wide range of underlying assets.
*   Exchange traded
*   Specifications need to be defined:
    *   What can be delivered,
    *   Where it can be delivered,
    *   When it can be delivered
*   Settled daily (Marked-to-market)

## Futures Contracts

*   Margin
    *   A margin is cash or marketable securities deposited by an investor with his or her broker.
        *   The balance in the margin account is adjusted to reflect daily settlement.
        *   Margins minimize the possibility of a loss through a default on a contract.
    *   Upon contract initiation, both parties open margin accounts.
    *   Associated with each type of contract is an initial margin and a maintenance margin.
        *   The initial deposit of funds into the margin account is known as initial margin.
        *   The maintenance margin is less than the initial margin.
    *   If the balance in your margin account falls below the maintenance margin, you will receive a margin call that requires you to increase your margin account back to the initial margin level.

## Futures Contracts

An investor takes a long position in December gold futures contracts on June 5
*   contract size is 100 oz.
*   futures price is US$400
*   margin requirement is US$2,000/contract (US$4,000 in total)
*   maintenance margin is US$1,500/contract (US$3,000 in total)

| Day     | Futures Price (US$) | Daily Gain (Loss) (US$) | Cumulative Gain (Loss) (US$) | Margin Account Balance (US$) | Margin Call (US$) |
| :------ | :------------------ | :---------------------- | :--------------------------- | :--------------------------- | :---------------- |
|         | 400.00              |                         |                              | 4,000                        |                   |
| 5-Jun   | 397.00              | (600)                   | (600)                        | 3,400                        | 0                 |
| :       | :                  | :                       | :                            | :                            | :                |
| :       | :                  | :                       | :                            | :                            | :                |
| 13-Jun  | 393.30              | (420)                   | (1,340)                      | 2,660 + 1,340 = 4,000        |                   |
|         |                     |                         |                              | < 3,000                      |                   |
| :       | :                  | :                       | :                            | :                            | :                |
| :       | :                  | :                       | :                            | :                            | :                |
| 19-Jun  | 387.00              | (1,140)                 | (2,600)                      | 2,740 + 1,260 = 4,000        |                   |
| :       | :                  | :                       | :                            | :                            | :                |
| :       | :                  | :                       | :                            | :                            | :                |
| 26-Jun  | 392.30              | 260                     | (1,540)                      | 5,060                        | 0                 |

## Futures Contracts

One orange juice futures contract is on 15,000 pounds of frozen concentrate. Suppose that on April 01, 2024, a company buys five September 2024 orange juice futures contracts for $1.20 per pound. In the following four days the price of the contract follows the following path: $1.12, $1.05, $1.15, and $1.40. Initial margin per contract is $4,500 and the maintenance margin is $3,000 per contract.

What is the company's profit or loss on the contract?
How does the margin account balance change between April 01, 2024, and April 05, 2024?

|        | \# of Contracts | Contract Size | Position | Futures Price | \$ Position | Daily Gain/Loss | Cumulative Gain/Loss | Margin Account Balance | Margin Call |
| :----- | :-------------- | :------------ | :------- | :------------ | :---------- | :-------------- | :------------------- | :--------------------- | :---------- |
| 1-Apr-24 | 5               | 15,000        | 75,000   | 1.20          | 90,000      |                 |                      | 22,500                 | 0           |
| 2-Apr-24 | 5               | 15,000        | 75,000   | 1.12          | 84,000      | -6,000          | -6,000               | 16,500                 | 0           |
| 3-Apr-24 | 5               | 15,000        | 75,000   | 1.05          | 78,750      | -5,250          | -11,250              | 11,250                 | 11,250      |
| 4-Apr-24 | 5               | 15,000        | 75,000   | 1.15          | 86,250      | 7,500           | -3,750               | 30,000                 | 0           |
| 5-Apr-24 | 5               | 15,000        | 75,000   | 1.40          | 105,000     | 18,750          | 15,000               | 48,750                 | 0           |

## Futures Contracts

A trader enters into a short cotton futures contract when the futures price is 50 cents per pound. The contract is for the delivery of 50,000 pounds. How much does the trader gain or lose if the cotton price at the end of the contract is (a) 48.20 cents per pound; (b) 51.30 cents per pound?

Payoff from a short position: $F – S_T$
$50,000 * (0.50 – 0.4820) = \$900$
$50,000 * (0.50 – 0.5130) = -\$650$

Suppose that you enter into a short futures contract to sell July silver for $27.20 per ounce. The size of the contract is 500 ounces. The initial margin is $4,000, and the maintenance margin is $3,000. What change in the futures price will lead to a margin call? What happens if you do not meet the margin call?

Contract Size $*(P_1 - P_0) \le$ (Maintenance Margin – Initial Margin)
$\Delta f \le (3000 – 4000)$
$500 * (P_1 – 27.20) \le (3000 – 4000)$
$P_1 \le 25.20$

A company enters into a short futures contract to sell 5,000 bushels of wheat for 450 cents per bushel. The initial margin is $3,000 and the maintenance margin is $2,000. What price change would lead to a margin call? Under what circumstances could $1,500 be withdrawn from the margin account?

$\Delta f \le (2000 – 3000)$
$5000 * (P_1 – 4.50) \le (2000 – 3000)$
$P_1 \le 4.30$

$\Delta f \ge 1500$
$5000 * (P_2 - 4.50) \ge 1500$
$P_2 \ge 4.80$

## Futures Contracts

*   Forward price for an investment asset
    $$F = S_0 e^{rT}$$
*   Forward price with known income
    $$F = (S_0 - I) e^{rT}$$
    *   Stocks paying known dividends and coupon-bearing bonds
*   Forward price with known yield
    $$F = S_0 e^{(r-q)t}$$
    *   a forward contract provides a known yield rather than a known cash income
*   Contracts on currencies
    $$F_{D/F} = S_{0,D/F} e^{(r_D-r_F)t}$$
*   Futures on commodities
    *   In the absence of storage costs and income
        $$F = S_0 e^{rT}$$
    *   Storage costs can be treated as negative income.
        $$F = (S_0 + U) e^{rT}$$
    *   If the net storage costs are proportional to the price of the commodity
        $$F = S_0 e^{(r+u)t}$$

## Futures Contracts

*   Long & Short Hedges
    *   A long futures hedge is appropriate when you know you will purchase an asset in the future and want to lock in the price.
    *   A short futures hedge is appropriate when you know you will sell an asset in the future & want to lock in the price.
*   Arguments in favor of hedging
    *   Companies should focus on the main business they are in and take steps to minimize risks arising from interest rates, exchange rates, and other market variables.
*   Arguments against hedging
    *   Shareholders are usually well diversified and can make their own hedging decisions.
    *   It may increase risk to hedge when competitors do not.
    *   Explaining a situation where there is a loss on the hedge and a gain on the underlying can be difficult.

## Swaps

*   A swap is an over-the-counter derivatives agreement between two companies to exchange cash flows in the future according to certain specified rules.
    *   The agreement defines the dates when the cash flows are to be paid and the way in which they are to be calculated.
    *   Usually, the calculation of the cash flows involves the future value of an interest rate, an exchange rate, or other market variable.
    *   Counterparty risk.
*   A forward contract can be viewed as a simple example of a swap.
    *   Whereas a forward contract is equivalent to the exchange of cash flows on just one future date, swaps typically lead to cash-flow exchanges taking place on several future dates.
*   Main types
    *   Interest rate swaps,
    *   Currency swaps,
    *   Credit default swaps.

## Swaps

*   Interest rate swaps
    *   The counterparties swap payments in the same currency based on an interest rate.
        *   An agreement by Arturu Corp to receive 6-month LIBOR and pay a fixed rate of 3% per annum every 6 months for 3 years on a notional principal of $100 million.
        *   This is a plain vanilla interest rate swap in which a company agrees to pay cash flows equal to interest at a predetermined fixed rate on a notional principal for a predetermined number of years. In return, it receives interest at a floating rate on the same notional principal for the same period of time.
        *   The floating interest rate is commonly referred to as the reference rate.
            *   The floating rate in most interest rate swap agreements is the London Interbank Offered Rate (LIBOR).
            *   It is the rate of interest at which a bank is prepared to lend money to other banks that have a AA credit rating.
            *   LIBOR rates are published each day for a number of different currencies, and several different borrowing periods ranging from overnight to one year.

## Swaps

Cash flows (millions of dollars) to Arturu Corp in a $100 million three-year interest rate swap when a fixed rate of 3% is paid and LIBOR is received

|            | 6-month LIBOR rate (%) | Floating cash flow received | Fixed cash flow paid | Net cash flow |
| :--------- | :--------------------- | :-------------------------- | :------------------- | :------------ |
| 1-Mar-21   | 2.80                   |                             |                      |               |
| 1-Sep-21   | 2.60                   | 1.40                        | 1.50                 | -0.10         |
| 1-Mar-22   | 2.40                   | 1.30                        | 1.50                 | -0.20         |
| 1-Sep-22   | 3.20                   | 1.20                        | 1.50                 | -0.30         |
| 1-Mar-23   | 3.60                   | 1.60                        | 1.50                 | 0.10          |
| 1-Sep-23   | 4.50                   | 1.80                        | 1.50                 | 0.30          |
| 1-Mar-24   |                        | 2.25                        | 1.50                 | 0.75          |

*   The principal itself is not exchanged.
    *   It is used only for the calculation of interest payments.
    *   Usually called the notional principal.

## Swaps

*   Microsoft agrees to pay Intel an interest rate of 5% per annum on a principal of $100 million, and in return Intel agrees to pay Microsoft the six-month LIBOR rate on the same principal.
    *   The swap can be used by Microsoft to switch its borrowings from floating to fixed and by Intel to do the reverse:

|                        | Microsoft    | Intel         |
| :--------------------- | :----------- | :------------ |
| Loan payment           | LIBOR + 0.1% | 5.2%          |
| Add: Paid under swap   | 5.0%         | LIBOR         |
| Less: Received under swap | -LIBOR       | -5.0%         |
| Net payment            | 5.1%         | LIBOR + 0.2%  |

    *   Microsoft can switch its assets from fixed to floating and Intel can do the reverse:

|                         | Microsoft    | Intel         |
| :---------------------- | :----------- | :------------ |
| Investment income       | 4.7%         | LIBOR – 0.2%  |
| Less: Paid under swap   | -5.0%        | -LIBOR        |
| Add: Received under swap | LIBOR        | 5.0%          |
| Net income              | LIBOR – 0.3% | 4.8%          |

## Swaps

*   Fixed-for-fixed Currency Swaps
    *   Involves exchanging principal and payments at a fixed rate of interest in one currency for principal and payments at a fixed rate of interest in another currency.
        *   The principal amount specified in each of the two currencies.
        *   The principal amounts are usually exchanged at the beginning and at the end of the life of the swap.
    *   A hypothetical five-year currency swap agreement between IBM and British Petroleum. IBM pays a fixed rate of interest of 5% in sterling and receives a fixed rate of interest of 6% in dollars from British Petroleum. Interest rate payments are made once a year and the principal amounts are $15 million and £10 million.
        *   At the outset of the swap, IBM pays $15 million and receives £10 million.
        *   Each year during the life of the swap contract, IBM receives $0.90 million (6% of $15 million) and pays £0.50 million (5% of £10 million).
        *   At the end of the life of the swap, it pays a principal of £10 million and receives a principal of $15 million.

## Swaps

*   Credit Default Swaps
    *   A credit default swap (CDS) is an OTC derivative that permits the buying and selling of credit protection against particular types of events that can adversely affect the credit quality of a bond such as the default of the borrower.
    *   There are two parties:
        *   Credit protection buyer
        *   Credit protection seller.
    *   The buyer of the insurance obtains the right to sell bonds issued by the reference entity for their face value when a credit event occurs and the seller of the insurance agrees to buy the bonds for their face value when a credit event occurs.
        *   The reference entity is a specific issuer (i.e. a company, a country).
        *   The specific credit-related events are identified in the contract that will trigger a payment by the credit protection seller to the credit protection buyer are referred to as credit events.

## Swaps

Spread Vietnam 10 Years / United States 10 Years Bond
(Graph showing spread from 2017 to 2024, with options for Zoom: 1m, 3m, 6m, YTD, 1y, All. Current view from 5 Sep 2016 to 6 May 2024.)

## Swaps

Sovereign CDS Spread

| Country       | Sovereign CDS Spread | Net of US | Country      | Sovereign CDS Spread | Net of US | Country           | Sovereign CDS Spread | Net of US | Country        | Sovereign CDS Spread | Net of US |
| :------------ | :------------------- | :-------- | :----------- | :------------------- | :-------- | :---------------- | :------------------- | :-------- | :------------- | :------------------- | :-------- |
| Abu Dhabi     | 0.70%                | 0.27%     | El Salvador  | 14.88%               | 14.45%    | Latvia            | 0.95%                | 0.52%     | Rwanda         | 5.19%                | 4.76%     |
| Algeria       | 1.59%                | 1.16%     | Estonia      | 0.91%                | 0.48%     | Lebanon           | NA                   | NA        | Saudi Arabia   | 0.89%                | 0.46%     |
| Angola        | 10.47%               | 10.04%    | Ethiopia     | 28.36%               | 27.93%    | Lithuania         | 0.95%                | 0.52%     | Senegal        | 5.39%                | 4.96%     |
| Argentina     | NA                   | NA        | Finland      | 0.26%                | 0.00%     | Malaysia          | 1.00%                | 0.57%     | Serbia         | 2.77%                | 2.34%     |
| Australia     | 0.33%                | 0.00%     | France       | 0.41%                | 0.00%     | Mexico            | 1.88%                | 1.45%     | Slovakia       | 0.54%                | 0.11%     |
| Austria       | 0.20%                | 0.00%     | Germany      | 0.22%                | 0.00%     | Morocco           | 1.95%                | 1.52%     | Slovenia       | 0.71%                | 0.28%     |
| Bahrain       | 3.16%                | 2.73%     | Greece       | 1.31%                | 0.88%     | Namibia           | 2.43%                | 2.00%     | South Africa   | 3.71%                | 3.28%     |
| Belgium       | 0.31%                | 0.00%     | Guatemala    | 2.42%                | 1.99%     | Netherlands       | 0.21%                | 0.00%     | Spain          | 0.79%                | 0.36%     |
| Brazil        | 2.88%                | 2.45%     | Hong Kong    | 0.54%                | 0.11%     | New Zealand       | 0.35%                | 0.00%     | Sri Lanka      | NA                   | NA        |
| Bulgaria      | 1.40%                | 0.97%     | Hungary      | 2.02%                | 1.59%     | Nicaragua         | 5.20%                | 4.77%     | Sweden         | 0.24%                | 0.00%     |
| Cameroon      | 6.45%                | 6.02%     | Iceland      | 0.81%                | 0.38%     | Nigeria           | 7.50%                | 7.07%     | Switzerland    | 0.28%                | 0.00%     |
| Canada        | 0.41%                | 0.00%     | India        | 1.42%                | 0.99%     | Norway            | 0.23%                | 0.00%     | Thailand       | 0.79%                | 0.36%     |
| Chile         | 1.47%                | 1.04%     | Indonesia    | 1.53%                | 1.10%     | Oman              | 2.00%                | 1.57%     | Tunisia        | 7.86%                | 7.43%     |
| China         | 1.00%                | 0.57%     | Iraq         | 4.80%                | 4.37%     | Pakistan          | NA                   | NA        | Turkey         | 5.05%                | 4.62%     |
| Colombia      | 3.54%                | 3.11%     | Ireland      | 0.36%                | 0.00%     | Panama            | 1.72%                | 1.29%     | Ukraine        | NA                   | NA        |
| Costa Rica    | 3.33%                | 2.90%     | Israel       | 0.80%                | 0.37%     | Peru              | 1.46%                | 1.03%     | United Kingdom | 0.40%                | 0.00%     |
| Croatia       | 1.12%                | 0.69%     | Italy        | 1.45%                | 1.02%     | Philippines       | 1.44%                | 1.01%     | United States  | 0.43%                | 0.00%     |
| Cyprus        | 1.14%                | 0.71%     | Japan        | 0.26%                | 0.00%     | Poland            | 1.02%                | 0.59%     | Uruguay        | 0.95%                | 0.52%     |
| Czech Republic | 0.45%                | 0.02%     | Kazakhstan   | 1.68%                | 1.25%     | Portugal          | 0.71%                | 0.28%     | Venezuela      | 11.57%               | 11.14%    |
| Denmark       | 0.19%                | 0.00%     | Kenya        | 7.85%                | 7.42%     | Qatar             | 0.71%                | 0.28%     | Vietnam        | 1.73%                | 1.30%     |
| Dubai         | 1.26%                | 0.83%     | Korea        | 0.41%                | 0.00%     | Romania           | 2.33%                | 1.90%     | Zambia         | NA                   | NA        |
| Egypt         | 13.19%               | 12.76%    | Kuwait       | 0.70%                | 0.27%     | Russia            | NA                   | NA        |                |                      |           |

As of July 2023

## Exercises

Suppose that you enter into a six-month forward contract on a non-dividend-paying stock when the stock price is $30 and the risk-free interest rate (with continuous compounding) is 12% per annum. What is the forward price?

$$F = S_0 e^{rT} = 30 * e^{0.12*0.5} = \$31.86$$

A one-year long forward contract on a non-dividend-paying stock is entered into when the stock price is $40 and the risk-free rate of interest is 10% per annum with continuous compounding.
*   What are the forward price and the initial value of the forward contract?
*   Six months later, the price of the stock is $45 and the risk-free interest rate is still 10%. What are the forward price and the value of the forward contract?

$$F = S_0 e^{rT} = 40 * e^{0.10*1} = \$44.21$$
$$F = S_0 e^{rT} = 45 * e^{0.10*0.5} = \$47.31$$
$$f = (F_0 - K)e^{-rT} = (47.31 – 40)e^{-0.10*0.05}= \$6.95$$
$f$: Value of contract; $F_0$: Forward price @ t = 1;
$K$: Delivery price in the contract

You enter into a forward contract to buy a 10-year, zero coupon bond that will be issued in one year. The face value of the bond is $1,000, and the 1-year and 11-year spot interest rates are 5 percent and 7 percent, respectively. What is the forward price of your contract?

$$S_0 = 1,000(1 + 0.07)^{-11}= 475.09$$
$$F = S_0(1 + r)^T = 475.09 * (1 + 0.05)^1 = 498.85$$

## Exercises

Consider a six-month forward contract on an asset that trades at $100 and is expected to provide income equal to 2% of the asset price once during a six-month period. The risk-free rate of interest with continuous compounding is 10% per annum. What should be the 6-month forward price contract on this asset?

$$(1 + 1/2)^2 = e^{rc}$$
$$e^{rc} = 3.96\%$$
$$F = S_0 e^{(r_f-r_c)T} = 100e^{(0.10-0.0396)*0.5} = \$103.07$$
vs.
$$F = S_0 e^{(r_f)T} = 100e^{0.10*0.5} = \$105.13$$

The current EUR/USD exchange rate is 1.4000 dollar per euro. The six-month forward exchange rate is 1.3950. The six-month USD interest rate is 1% per annum, compounded continuously. Estimate the six-month euro interest rate.

$$F(\text{USD per EUR}) = S_0(\text{USD per EUR}) * \frac{e^{r_{\text{US}}T}}{e^{r_{\text{EUR}}T}}$$
$$1.3950 * e^{r_{\text{EUR}}*0.05} = 1.40 * e^{0.01*0.05}$$
$$r_{\text{Euro}} = 0.17156\%$$

Replication: Borrow €100,000 @0.1716%, Exchange @ 1.40 €/$, Invest $140,000 @1%, Receive $140,701.75, Deliver $140,701.75 for €100,861.47, Pay back €100,861.47.

## Exercises

The spot exchange rate between the Euro and U.S. dollar is 1.0800(EUR/USD). Interest rates in the U.S. and Euro Area are 4.0% and 2.0% per annum, respectively, with continuous compounding. The three-month forward exchange rate is 1.1000 (EUR/USD).
*   What arbitrage strategy is possible?
*   How does your answer change if the forward exchange rate is 1.0600 (EUR/USD).

|                   | FWD @ 1.10 EUR/USD |           | FWD @ 1.06 EUR/USD |           |
| :---------------- | :----------------- | :-------- | :----------------- | :-------- |
|                   | Today              | 3-months  | Today              | 3-months  |
| **EUR**           |                    |           |                    |           |
| Borrow            |                    |           | 100,000.00         | -100,501.25 |
| Exchange          | 92,592.59          |           | -100,000.00        |           |
| Invest            | -92,592.59         | 93,056.71 |                    |           |
| Net               | 0.00               | 93,056.71 | 0.00               | -100,501.25 |
| **USD**           |                    |           |                    |           |
| Borrow            | 100,000.00         | -101,005.02 |                    |           |
| Exchange          | -100,000.00        |           | 108,000.00         |           |
| Invest            |                    |           | -108,000.00        | 109,085.42 |
| Net               | 0.00               | -101,005.02 | 0.00               | 109,085.42 |
| **Forward**       |                    |           |                    |           |
| EUR               |                    |           |                    |           |
| Deliver           |                    | -93,056.71 |                    |           |
| Receive           |                    |           |                    | 100,501.25 |
| USD               |                    |           |                    |           |
| Deliver           |                    |           |                    | -106,531.27 |
| Receive           |                    | 102,362.38 |                    |           |
| **Overall**       |                    |           |                    |           |
| EUR               | 0.00               | 0.00      | 0.00               | 0.00      |
| USD               | 0.00               | 1,357.36  | 0.00               | 2,554.15  |

*   When forward EUR/USD is @ 1.10:
    *   Sell FWD EUR/USD @ 1.10
    *   Borrow USD, Exchange USD for EUR @ 1.08
    *   Invest EUR
    *   Deliver EUR, Receive USD
*   When forward EUR/USD is @ 1.06:
    *   Buy FWD EUR/USD @ 1.06
    *   Borrow EUR, Exchange EUR for USD @ 1.08
    *   Invest USD
    *   Deliver USD, Receive EUR

## Exercises

Suppose that the six-month CAC futures contract trades at 5,000. The interest rate is 1% per year and the dividend yield on the index is 2.8%. What should be the no arbitrage level of index currently?

$$F = 5,000 = S_0(1 + r - y)^t= S_0(1 + 0.005 – 0.014)$$
$$S_0 = 5,045.41$$

Calculate the value of a six-month futures contract on a Treasury bond. You have the following information:
*   Risk-free interest rate: 10% (EAR)
*   Spot price of bond: $95.
*   The bond pays a 4% coupon every six months.

$$F = S_0(1 + r - y)^t= 95(1 + 0.0488 – 0.04) = \$95.84$$

The spot price of crude oil was $57.57 a barrel and the six-month futures price is $56.91 per barrel. The effective interest rate is 2.4% per year. What is the net convenience yield?

$$F = 56.91 = S_0(1 + r + c − y)^t= 57.57(1 + 0.012 + c − 0)$$
$$c_{\text{Annual}} = (1 + 0.0235)^2 = 4.75\%$$

## Exercises

You are a dealer in kryptonite and are contemplating a trade in a forward contract. You observe that the current spot price per ounce of kryptonite is $180.00, the forward price for delivery of one ounce of kryptonite in one year is $205.20, and annual carrying costs of the metal are 4% of the current spot price.
*   What is the annual return on a riskless zero-coupon security implied by the Law of One Price?
*   Identify a trading strategy that would generate arbitrage profits for you if the annual return on the riskless security is 5%? What would your arbitrage profit be, per ounce of kryptonite?

$$F = 205.20 = S_0(1 + r + c − y)^t= 180(1 + r + 0.04 – 0)$$
$$r = 10\%$$
$$F = S_0(1 + r + c − y)^t= 180(1 + 0.05 + 0.04 – 0) = 196.20$$
Sell FWD, Borrow 195.43, Buy @ Spot, Deliver in 1 year, receive 205.20, Pay back debt of 205.20.

Assume the current spot price of the South African rand is $0.0995 and the one-year forward price is $0.0997. If the riskless annual dollar interest rate is 5%, what is the implied riskless annual rand interest rate?

$$F_0\left(\frac{\text{Rand}}{\text{USD}}\right) = S_0\left(\frac{\text{Rand}}{\text{USD}}\right) \frac{(1 + r_{\text{USD}})}{(1 + r_{\text{Rand}})}$$
$$0.0997 = 0.0995 \frac{(1 + 0.05)}{(1 + r_{\text{Rand}})}$$
$$r_{\text{Rand}} = 4.7894\%$$

## What is next?

*   Derivatives II
    *   Introduction to options
    *   Option Payoffs
    *   Put-Call Parity
    *   Factors Affecting Option Prices
    *   Reading(s): BKM: Ch. 21
    *   Suggested Problems:
        *   Ch. 22: 12, 13.
        *   Ch. 22-CFA Problems: 1, 4.
        *   Ch. 23: 5, 7, 12, 15, 18.
        *   Ch. 23-CFA Problems: 5, 8.
```