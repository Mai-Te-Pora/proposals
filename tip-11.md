# Additional Markets and Pool Weight Adjustments

## Intro

It has been more than one month since the new Binance Smart Chain markets and pool weights were introduced via [TIP-10](https://forum.switcheo.foundation/topic/61/tip-10-extension-of-lp-rewards-updating-of-pool-weights/19). This proposal included several NEO pairs, however these have not yet been added due to NEO3 scheduling.

## About me

I am a validator, trader and liquidity provider, but most importantly, I am a (bot) developer. Immediately after the the launch of demex, I began trading and have never stopped since then.
Currently I run trading bots on Demex and produce a few million dollars of volume per month and I am in the top 10 of the trading leaderboard. Analysing and optimizing is part of my botting business/hobby.
The changes, additions and adjustments I propose below will definitly not only benifit me, but also other traders. Which benefits the stakers in the end via increased volume, fees and platform awareness.

It is important to me that I am transparent about my motives and the proposed changes.

## Missing Markets

Currently these missing markets are waiting be launched with NEO3.

- GAS/NNEO
- NEX/NNEO

## Current Markets

In the following section, I review the existing Demex markets and provide my view of why the markets are currently performing the way they do, with emphesis on arbitrage possibilities.

### ETH/USDC , SWTH/USDC and SWTH/ETH

Three of the main markets since launch. The performance of all three has been good. People want to buy SWTH to stake or convert their staking profits into different assets.
ETH prices have performed well in the last months and has therefore also been a good performer.

Takin a closer look at these 3 markets, they build an triangular arbitrage oppurtunity. Due to this a huge amount of the past weeks volume was produced by my bot.
Arbitrage means that if one of the three pairs changes price, the other two must also change. For example if ETH increases in price, the price in the SWTH/ETH has to decrease, otherwise the price for USDC/SWTH will not match the value in ETH.
Such opportunity occurs all the time since the markets flucturates a lot.

### ETH/USDC , WBTC/USDC and ETH/WBTC

These three markets create another triangular arbitrage opportunity, however the performance is not as good as USDC/ETH/SWTH. This is because BTC and ETH behave similarly, most commonly moving in the same direction, however sometimes one does perform better/worse.
One reason these markets perform quite well is because the WBTC/USDC markets offers opportunities for cross exchange arbitrage. Deposits and withdrawals of WBTC, as for all ERC-20 tokens, are currently really expensive.

### BUSD/USDC

Probobly one of the most important markets (for me) on Demex. This market is a bridge between all USDC and BUSD pairs and creates a lot of new triangular opportunites and generates a lot of demex volume.

The best example is USDC/BUSD + BUSD/SWTH + USDC/SWTH. At the time of creating the BUSD markets switcheo had a listing event with Pancake Swap. This caused a huge price increase. Best thing was that deposits and withdrawals of BUSD and SWTH(BSC) are really really cheap and fast.
Because of this triangular arbitrage the USDC/BUSD market crashed from 1 / 1 to 1 / 0.88, this means with 0.88 USDC it was possible to buy one full BUSD. But this is just one reason this market crashed. The second one is the AMM protocol from DEMEX.
This protocol defines how the pools are transformed to orderbooks. We already saw adjustments on the protocol. But one main issue is that algorithm is not designed to work with 1 to 1 pools like BUSD/USDC or BTCB/WBTC. The large maker orders of these market are far from the match point, which require large slippage (for a stable coint), therefore they are not used.
The main reason for this behaviour is to protect liquidity providers. In my opinion BUSD/USDC and BTCB/WBTC are every safe markets and therfore should use more of the pool volume at closer to the match point.

### NNEO/USDC NNEO/BUSD and CEL/USDC CEL/BUSD

With the release of the new markets the pool weight of NNEO/USDC and CEL/USDC was removed. These pools are now almost empty and provide really bad liquidity. With the new BUSD/USDC market there is now triangular arbitrage opportunites which cannot be used due to this lack of liquidity.
In my opinion these markets need new pool weights to restore some volume.

### NNEO/ETH

A good market creates a triangular arbitrage opportunity, but with low liquidity NNEO/USDC limits volume.

### BTCB/WBTC

Honestly this pair just has liquidity because of the pool weight and is a safe haven. Currently there is no good (triangular or cross exchange) arbitrage possible. We need more pairs with BTCB like BTCB/BUSD which would provide new triangular arbitrage opportunities with WBTC/USDC and BUSD/USDC.

### NEX/USDC

Not bad at all, but only NEX/USDC is available at the moment. It is expensive to do arbitrage in my opinion.

### BNB/ETH

The forgotten child. No liqudity, no pool weight and no arbitrage opportunity.

## Current Triangular Arbitrage Opportunities

In summary, here are the existing on-exchange arbitrage opportunities

### BUSD1

- BUSD1-CEL1-USDC1-BUSD1
- BUSD1-NNEO2-USDC1-BUSD1
- BUSD1-SWTH-USDC1-BUSD1
- BUSD1-USDC1-CEL1-BUSD1
- BUSD1-USDC1-NNEO2-BUSD1
- BUSD1-USDC1-SWTH-BUSD1

### CEL1

- CEL1-BUSD1-USDC1-CEL1
- CEL1-USDC1-BUSD1-CEL1

### BNB1

None

### BTCB

None

### ETH1

- ETH1-NNEO2-USDC1-ETH1
- ETH1-SWTH-USDC1-ETH1
- ETH1-USDC1-NNEO2-ETH1
- ETH1-USDC1-SWTH-ETH1
- ETH1-USDC1-WBTC1-ETH1
- ETH1-WBTC1-USDC1-ETH1

### NNEO2

- NNEO2-BUSD1-USDC1-NNEO2
- NNEO2-ETH1-USDC1-NNEO2
- NNEO2-USDC1-BUSD1-NNEO2
- NNEO2-USDC1-ETH1-NNEO2

### SWTH

- SWTH-BUSD1-USDC1-SWTH
- SWTH-ETH1-USDC1-SWTH
- SWTH-USDC1-BUSD1-SWTH
- SWTH-USDC1-ETH1-SWTH

### USDC1

- USDC1-BUSD1-CEL1-USDC1
- USDC1-BUSD1-NNEO2-USDC1
- USDC1-BUSD1-SWTH-USDC1
- USDC1-CEL1-BUSD1-USDC1
- USDC1-ETH1-NNEO2-USDC1
- USDC1-ETH1-SWTH-USDC1
- USDC1-ETH1-WBTC1-USDC1
- USDC1-NNEO2-BUSD1-USDC1
- USDC1-NNEO2-ETH1-USDC1
- USDC1-SWTH-BUSD1-USDC1
- USDC1-SWTH-ETH1-USDC1
- USDC1-WBTC1-ETH1-USDC1

### WBTC1

- WBTC1-ETH1-USDC1-WBTC1
- WBTC1-USDC1-ETH1-WBTC1

## New Markets

The following list represents pairs which could fill a gap and provide new opportunities.

### CEL/ETH

WTF why is this pair not on demex yet?

### SWTH/NEO

Main market from switcheo exchange, I miss this market );

### SWTH/BTCB

First BTC pair with SWTH. I suggest BTCB because it is cheaper and allows directly arbitrage with Pancake Swap.

### BTCB/BUSD

Equivalent to WBTC/USDC a new BSC pair with cheap deposit and withdrawal. This could help arbitraging the ERC pairs.

### BNB/BUSD

This market could bring good volume too since Binance burns BNB on a regular basis.

## Proposal
I propose to list the following markets: *CEL/CEL* and *BNB/BUSD*. Regarding *SWTH/BTC*, *BTCB/BUSD* and *SWTH/NEO* I would like to hear opinions.

These new pool weights I suggest(if all markets get listed):

| Market    | Cur. Pool weight | New Pool weight | Liquidity | 24H Volume |
|-----------|------------------|-----------------|-----------|------------|
| SWTH/ETH  | 4 - 20%          | 15 - 15%        | $5.45m    | $783,733   |
| WBTC/BTCB | 1 - 5%           | 2 - 2%          | $2.70m    | $15,078    |
| SWTH/USDC | 4 - 20%          | 15 - 15%        | $2.67m    | $338,594   |
| WBTC/USDC | 2 - 10%          | 7 - 7 %         | $2.10m    | $113,515   |
| ETH/WBTC  | 1 - 5%           | 5 - 5%          | $2.10m    | $71,889    |
| USDC/BUSD | 1 - 5%           | 3 - 3%          | $1.99m    | $109,226   |
| ETH/USDC  | 2 - 10%          | 8 - 8%          | $1.65m    | $343,956   |
| ETH/nNEO  | 1 - 5%           | 4 - 4%          | $1.22m    | $62,582    |
| nNEO/BUSD | 1 - 5%           | 4 - 4%          | $839,129  | $99,801    |
| SWTH/BUSD | 2 - 10%          | 8 - 8%          | $623,983  | $99,046    |
| CEL/BUSD  | 1 - 5%           | 3 - 3%          | $552,435  | $14,187    |
| nNEO/USDC | 0 - 0%           | 4 - 4%          | $59,160   | $37,371    |
| NEX/USDC  | 0 - 0%           | 0 - 0%          | $10,886   | $28        |
| CEL/USDC  | 0 - 0%           | 3 - 3%          | $4375     | $192       |
| ETH/BNB   | 0 - 0%           | 8 - 8%          | $0        | $0         |
| BNB/BUSD  | -                | 8 - 8%          | -         | -          |
| ETH/CEL   | -                | 3 - 3%          | -         | -          |
| SWTH/BTCB | -                | 3 - 3%          | -         | -          |
| BTCB/BUSD | -                | 4 - 4%          |           |            |
| SWTH/nNEO | -                | 3 - 3%          | -         | -          |

*Liquidity and 24 volmues taken from [Demex](https://app.dem.exchange/pools) - 04-27-2021*

I tried to not make the changes too drastic, like removing all pool weight. I think the bigger pools are quite good and can share a bit of their weight. Some could now say that there are up to 25% decrease, yes but I used this decrease to boost mainly new SWTH markets or BSC markets. I also used 100 pool weights to adjust the weight at a 1% precision.

As you may have noticed, I have  not proposed new tokens, because I think we can still improve the liquidity a lot by improving the conditions.

I hope for a civilized discussion about my proposed changes, I am open for feedback and changes as well.

Devel
