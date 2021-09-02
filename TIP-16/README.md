# Intro
All data shown in this thread wa collected from `2021-05-13 19:00:27.51635566 UTC +0:00`, the time the last adjustment took place and includes data until `2021-08-28 23:59:59.99999999 UTC +0:00` to make a clean daily cut.

Data can be accessed [here](https://docs.google.com/spreadsheets/d/1SJUyJ-5Tx3GYr-LTh_bThrS8L77fBU0shnOUHLQo07c/edit?usp=sharing).

This proposal consists of three sub-proposals:

* Extension of the Liquidity Provider rewards
* New Parterships Boost
* Pool weight adjustment

They impact each other and therefore I put them into one thread but will be executed in several steps on chain, if passed.

# Extension of the Liquidity provider rewards
The obvious first, which is a requirement for the next proposed steps. In my opinion there us no way around this to keep the markets tradable.

* Extend LP rewards to 30% of inflation value for 6 months, decreasing linearly each week to 20% for the last week.

Maybe higher since the value of SWTH dropped a lot. 

# New Partnership Boost

In order to get new users to Tradehub/Demex I suggest offering new projects a quite high boost for their markets. I propose to take 5 points equal to 5% total boost for new partnerships as long as they/or their community provide a certain amount of liquidity among all pairs including their token/coin. 
Furthermore, a time limitation of 30 days ensure that new projects have a chance to get a good boost for their project. In my opinion project will only chose Demex as their preferred exchange if we provide them good reasons too. In exchange we aquire new and fresh users to Tradehub.

I suggest following conditions to obtain the boost:
* min. Liquidity among all pairs: $100,000.00
* min. Liquidity per pool: $50,000.00
* Telegram + Twitter promotion to their user base

This is what I see we offer them:
* Exchange with orderbooks (Market, Limit, Stop, ...)
* High ARP since the provided Liquidity will be low compared to the received boost
* Support for the listing process(Validators already showed their willingness to create and fund the proposals)

If no other projects qualified for the next promotion month the boost can be removed/lowered or extended.

I am open for feedback and suggestions. 

# Pool weight adjustment

![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Demex%20Spot%20Volume.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Liquidity%20Total.png?raw=true)

The following table shows each market, and their total volume share. This indicates important markets for Demex. As a help the current boost and the liquidity is added to the table.
An important ratio is the Volume per Liquidity, this indicates how much Volume($) was generated per Liquidity($). A high ratio may say that this market had could make way more volume if more liquidity would have been provided.
Low ratios may say that this market would have done almost the same volume with less liquidity.

|           Market |         Volume |  Share | Boost |  Liquidity | Volume/Liquidity | New Boost |   Change |
|-----------------:|---------------:|-------:|------:|-----------:|-----------------:|----------:|---------:|
|       swth_usdc1 |  $7.004.444,98 | 18,61% | 18    | $1,280,000 | 5,47             |        16 |  -11,11% |
|       eth1_usdc1 |  $6.853.856,31 | 18,21% | 8     | $423,190   | 16,20            |        17 |  112,50% |
|       swth_busd1 |  $3.861.731,56 | 10,26% | 8     | $374,931   | 10,30            |         8 |    0,00% |
|        swth_eth1 |  $2.952.430,43 |  7,84% | 18    | $846,238   | 3,49             |         0 | -100,00% |
|      busd1_usdc1 |  $2.760.363,42 |  7,33% | 3     | $554,287   | 4,98             |         0 | -100,00% |
|      nneo2_busd1 |  $2.409.928,00 |  6,40% | 4     | $160,433   | 15,02            |        11 |  175,00% |
|       bnb1_busd1 |  $2.338.213,53 |  6,21% | 6     | $250,985   | 9,32             |         8 |   33,33% |
|      wbtc1_usdc1 |  $1.834.235,20 |  4,87% | 7     | $527,708   | 3,48             |         6 |  -14,29% |
|       nneo2_eth1 |  $1.450.589,42 |  3,85% | 4     | $259,523   | 5,89             |         4 |    0,00% |
|       eth1_wbtc1 |  $1.139.439,94 |  3,03% | 4     | $629,206   | 1,81             |         4 |    0,00% |
|      nneo2_usdc1 |    $968.479,93 |  2,57% | 2     | $72,303    | 13,39            |         5 |  150,00% |
|        bnb1_eth1 |    $934.906,48 |  2,48% | 6     | $356,704   | 2,62             |         5 |  -16,67% |
|      btcb1_busd1 |    $877.366,82 |  2,33% | 4     | $350,795   | 2,50             |         4 |    0,00% |
|       cel1_busd1 |    $827.083,73 |  2,20% | 3     | $155,276   | 5,33             |         4 |   33,33% |
|       cel1_usdc1 |    $552.667,65 |  1,47% | 2     | $127,110   | 4,34             |         0 | -100,00% |
|          cel_eth |    $549.008,77 |  1,46% | 2     | $114,556   | 4,79             |         3 |   50,00% |
|      wbtc1_btcb1 |    $242.671,12 |  0,64% | 1     | $285,182   | 0,85             |         0 | -100,00% |
|       nex1_usdc1 |     $15.295,22 |  0,04% | 0     | $1,372     | 11,15            |         0 |    0,00% |
| NEW Partnerships | -              | -      | -     | -          |                  | 5         | -        |
|                  | $37.638.287,28 |        | 100   |            |                  | 100       |          |


![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/AMM%20Volume%20_%20Liquidity%20Ratio.png?raw=true)
This diagram shows the ratio between the effective AMM volume divided by the liquidity in USD. For example the pair swth_usdc1 has a ratio of 3.89%.
The ratio tells how much volume was produced by the available liquidity over this time. The total AMM volume for swth_usdc1 (SUM Daily Volume) was $6.495.149,00, the total available liquidity(SUM Daily Liquidity Value) was $166.806.223,99.
With other words the ratio is the daily average relative volume against the available liquidity. The higher the ratio the more volume the pair produced.
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/AMM%20Volume%20_%20Liquidity%20Ratio%20per%20Boost%20Weight.png?raw=true)
This diagram takes the boost weight into consideration. It simply divides the ratio by the current pool weight. The result says how much volume was produced on daily average per boost weight.
A high ratio indicates that this pair could be doing way more daily volume if there would be more liquidity in the pool.
A low number on the other hand indicates that the pool is performing not that well. The reason has to be investigated.

## Explanation

### eth1_usdc1
As second most important trading pair a boost of 8% seems quite less. A closer look on the pool shows that this market has a really low liquidity compared to the total volume. This pair has the highest Volume/Liquidity ratio and indicates that we should increase the boost for this pair significantly.

Boosting this market may lead to a significant increase in daily volume. Especially after EIP-1559 has passed, which causes a burn on each block.

### swth_eth1
This market has the second biggest Liquidity pool but is performing pretty bad with an Volume/Liquidity ratio of 3,49 and a total boost of 18 points. As already suggested in the comments below it is worth to consider dropping the whole boost for this market and promote it external.

### busd1_usdc1
A perfect example for a successful market. A close look at the Market Maker Share shows that this market is almost 100% made by user orders. Due to this fact and that the AMM does not work very well with a stable coin pair removing the boost should not have any impact on the liquidity.

### nneo2_busd1 and nneo2_usdc1
It is insane how much volume those two markets generated with that low liquidity. nneo2_busd1 has a Volume/Liquidity ratio of 15,02 and nneo2_usdc1 13,39. Taking this into consideration these two pairs may do way more volume if they would feature more Liquidity.

On the other hand 3 pairs for Neo seems to much right now. Would like to hear more feedback from the community. In my opinion BUSD/NEO is preferred, it is way cheaper to trade across exchanges.

### bnb1_busd1 and bnb1_eth1
bnb1_busd1 performed pretty well. There is still potential upwards. Lowering bnb1_eth1 may shift liquidity to bnb1_busd1.

### CEL pairs
The cel pairs performed not that bad, but focusing on one or two pairs could make the deal here.

### wbtc1_btcb1
Not much to say, this pair should be no longer boosted.

# Market insights
Each market has three diagrams. Each diagram uses the same time duration.

Volume: Shows the daily absolute volume over the period.

Market Maker Shares - AMM vs. Users: Shows the daily relative maker matched volume over the period. This chart inidcates if an AMM is required for this market or not.

Volume Share: Shows the relative total daily volume over the period.
## swth_usdc1
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20swth_usdc1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Market%20Maker%20Shares%20swth_usdc1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20Share%20swth_usdc1.png?raw=true)
## eth1_usdc1
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20eth1_usdc1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Market%20Maker%20Shares%20eth1_usdc1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20Share%20eth1_usdc1.png?raw=true)
## swth_busd1
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20swth_busd1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Market%20Maker%20Shares%20swth_busd1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20Share%20swth_busd1.png?raw=true)
## swth_eth1
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20swth_eth1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Market%20Maker%20Shares%20swth_eth1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20Share%20swth_eth1.png?raw=true)
## busd1_usdc1
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20busd1_usdc1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Market%20Maker%20Shares%20busd1_usdc1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20Share%20busd1_usdc1.png?raw=true)
## nneo2_busd1
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20nneo2_busd1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Market%20Maker%20Shares%20nneo2_busd1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20Share%20nneo2_busd1.png?raw=true)
## bnb1_busd1
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20bnb1_busd1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Market%20Maker%20Shares%20bnb1_busd1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20Share%20bnb1_busd1.png?raw=true)
## wbtc1_usdc1
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20wbtc1_usdc1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Market%20Maker%20Shares%20wbtc1_usdc1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20Share%20wbtc1_usdc1.png?raw=true)
## nneo2_eth1
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20nneo2_eth1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Market%20Maker%20Shares%20nneo2_eth1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20Share%20nneo2_eth1.png?raw=true)
## eth1_wbtc1
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20eth1_wbtc1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Market%20Maker%20Shares%20eth1_wbtc1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20Share%20eth1_wbtc1.png?raw=true)
## nneo2_usdc1
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20nneo2_usdc1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Market%20Maker%20Shares%20nneo2_usdc1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20Share%20nneo2_usdc1.png?raw=true)
## bnb1_eth1
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20bnb1_eth1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Market%20Maker%20Shares%20bnb1_eth1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20Share%20bnb1_eth1.png?raw=true)
## btcb1_busd1
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20btcb1_busd1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Market%20Maker%20Shares%20btcb1_busd1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20Share%20btcb1_busd1.png?raw=true)
## cel1_busd1
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20cel1_busd1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Market%20Maker%20Shares%20cel1_busd1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20Share%20cel1_busd1.png?raw=true)
## cel1_usdc1
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20cel1_usdc1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Market%20Maker%20Shares%20cel1_usdc1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20Share%20cel1_usdc1.png?raw=true)
## cel_eth
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20cel_eth.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Market%20Maker%20Shares%20cel_eth.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20Share%20cel_eth.png?raw=true)
## wbtc1_btcb1
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20wbtc1_btcb1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Market%20Maker%20Shares%20wbtc1_btcb1.png?raw=true)
![](https://github.com/Mai-Te-Pora/proposals/blob/main/TIP-16/diagrams/Volume%20Share%20wbtc1_btcb1.png?raw=true)