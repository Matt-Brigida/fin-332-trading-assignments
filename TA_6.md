## FIN 332: Trading Assignment 6

Complete the following trades in your IB account and report your trade prices and times.  Also answer the questions below.  Upload your answers to the BB dropbox.  All futures contracts in this trading assignment can be found on the [CME website](https://www.cmegroup.com/).

Note that delivery months differ from one commodity to the next, and most products do not list all twelve months.  Check the contract specifications on the CME website before you trade, and **state which contract month you used for each trade below**.

1.  Sell 3000 barrels of crude oil (West Texas Intermediate) for delivery roughly six months from now.  How many contracts is this (and for what ticker)?  What is the delivery point?

2.  Buy 2 SOFR futures contracts.  Will your contracts gain in value when SOFR rates increase or decrease?

3.  Trade (buy or sell) Soybeans for delivery at least six months from now.  Soybeans are not listed for every month---which months are listed, and which did you choose?  How many bushels have you traded?  When is the last trading day for your contract?

4.  Trade Copper for delivery at least three months from now.  Which copper delivery months carry the most volume and open interest, and how can you tell?  When you enter into the contract what is the open interest, and what does open interest mean?

5.  Buy 4 E-mini S&P 500 futures contracts for the next quarterly delivery month.  Which four months does this contract use each year?  What is the multiplier on each contract, and how much of the S&P 500 have you bought (in $)?

6.  Buy 1 Euro FX futures contract for the next quarterly delivery month.  What is the contract size in euros, and what is the tick size?  What is the total dollar value of your position?

7.  Sell 1 Japanese Yen futures contract for the next quarterly delivery month.  Look carefully at how this contract is quoted---how is it different from the way you normally see the dollar/yen exchange rate quoted?

## Covered Interest Rate Parity

In TA 3 you saw that two currencies with different interest rates cannot both be a fair bet at today's exchange rate.  The currency futures price you just observed in question 6 is a *forward* price, and no-arbitrage ties it to the spot rate and to the two countries' interest rates:

```
F = S * (1 + r_d * T) / (1 + r_f * T)
```

where `S` is the spot rate in USD per euro, `F` is the forward (futures) price, `r_d` is the annualized US interest rate, `r_f` is the annualized euro area rate, and `T` is the time to delivery in years.

Using your Euro FX trade from question 6:

1.  Record `S`, the spot USD/EUR rate at the time of your trade, and `F`, your actual fill price on the futures contract.  Record `T`, the time to delivery in years.

2.  Look up `r_d` and `r_f`.  Use the 3-month government bill yield for each, and note the source and the date you retrieved it.

3.  Compute the CIP-implied forward rate and compare it to the futures price at which you actually traded.  How close are they?

4.  If your two numbers differ, then in principle there is an arbitrage.  Write out the sequence of trades you would make to capture it: what you borrow, what you convert, where you invest, and what you lock in with the futures contract.

5.  Now explain why you could not actually earn this profit.  Consider the bid/ask spread, the difference between your fill and the midpoint, the fact that you cannot borrow or lend at the government bill rate, and the margin you must post on the futures contract.

6.  Is the euro trading at a forward premium or a forward discount against the dollar?  Which of the two currencies has the higher interest rate?  State the general rule connecting the two.

## Hedging with Currency Futures

Suppose you are a US firm that expects to receive **1,000,000 euros** three months from now, and you want to lock in the dollar value today.

1.  Using the contract size from question 6, how many Euro FX futures contracts do you need, and do you buy or sell them?

2.  At the futures price you recorded, what dollar amount have you locked in?

3.  Build a small table showing your dollar proceeds if the spot rate at delivery is 5% above, equal to, and 5% below today's spot rate---both hedged and unhedged.  In which scenario does the hedge cost you money?  Was the hedge therefore a mistake?



<!-- ignore -->
<!-- 5.  Sell 2 10-year Treasury note futures contracts for the next quarterly delivery month.  For each contract, what is the contract size, what must be delivered, and what is the minimum tick size? -->
