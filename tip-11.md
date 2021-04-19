# Additional Markets and Pool Weight Adjustments
## Into
Since more than one month the new Binance Smart Chain markets and pool weights, introduced with [TIP-10](https://forum.switcheo.foundation/topic/61/tip-10-extension-of-lp-rewards-updating-of-pool-weights/19) are live. Due to NEO3 is not ready few markets are not ready yet.

Convention about the markets, since I already saw a few formations I will stick to BASE_ASSET / QUOTE_ASSET.

Example

60000 USD / BTC - spoken : 60000 USD per BTC : Market -> USD/BTC.

Exchanges display the markets quite often in this formation: QUOTE_ASSET / BASE_ASSET. Demex as well is using this formation to group the markets. The example above would be BTC / USD.

## About me
I am a validator, trader and liquidity provider, but most important I am a (bot) developer. In the very first minutes of the launch of demex I began trading and never stopped since then.
Currently I run trading bots on Demex and producing a few million $ volume per month and I am in the top 10 of the trading leaderboard. Analysing and optimizing is part of my botting business/hobby.
Changes, additions and adjustments I propose will definitly benifit me, but also other traders. Which benefits the stakers in the end.

It is important to me that I am transparent about me and the proposed changes.

## Missing Markets
Currently these missing markets are waiting be launched with NEO3.
+ NNEO / GAS
+ NNEO / NEX 

## Current Markets
I will speak a bit about the best and worst markets on demex to give (my) explaination why the markets perform how they do.

### USDC/ETH , USDC/SWTH and ETH/SWTH
Three of the main markets since launch. The performance of all three was always good. People want to buy SWTH to stake or convert their staking profits into different assets.
ETH did pretty well the last months and theirefore a good performed market too.

This is the first overview which most of the users would suggest. Now to take a close look, these three markets build an triangular arbitrage oppurtunity. Due to this a huge amount of the past weeks volume was produced by my bot.
This means if one of the three pairs changes the other two have to change too. For example if ETH increases in price the price in the ETH/SWTH has to decrease, otherwise the price for SWTH/USDC will not match the value in ETH.
Such opportunity occures all the time since the markets flucturates a lot. 

 ### USDC/ETH , USDC/WBTC and WBTC/ETH
 These three markets create another triangular arbitrage opportunity. The performance is not as good as the one mentioned before. This is because BTC and ETH are quite similar if one changes the other changes too. Sometimes one does perform better/worse.
 One reason these markets perform quite well is because the USDC/WBTC markets offers normal cross exchange arbitrage quite often. Deposits and withdrawals of WBTC, on all other ERC-20 tokens, are really expensive.
 
 ### USDC/BUSD
 Properly one of the most important markets (for me) on Demex. This market is a bridge between all USDC and BUSD pairs and creates a lot new triangular opportunites an generates still alot of demex volume.
 
 The best example is USDC/BUSD + BUSD/SWTH + USDC/SWTH. At the time of creating the BUSD markets switcheo had an listing event with Pancake Swap. This caused a huge price increase. Bets thing was that deposits and withdrawals of BUSD and SWTH(BSC) are really really cheap and fast.
 Because of this triangular arbitrage the USDC/BUSD market crashed from 1 / 1 to 1 / 0.88, this means with 0.88 USDC it was possible to buy one full BUSD. But this is just one reason this market crashed. The second one is the AMM protocol from DEMEX.
 This protocol defines how the pools are transformed to orderbooks. We already saw adjustments on the protocol. But one main issue is that algorithm is not supposed to work with 1 to 1 pools like  USDC/BUSD or WBTC/BTCB. The main volume of these pairs are almost unreachable not therefore not used.
 The main reason for this is to protect liquidity providers. In my opinion USDC/BUSD and WBTC/BTCB are every save markets and should use way more volume of their pool.
 
 ### USDC/NNEO BUSD/NNEO and USDC/CEL BUSD/CEL
 With the release of the new markets the pool weight of USDC/NNEO and USDC/CEL was removed. Now these pools are almost empty and provide really bad liquidity. With the new USDC/BUSD market there is now triangular arbitrage opportunites which can not be used due to the lack of liquidity.
 In my opinion these markets need new pool weights to get a bot of the volume back.
 
 ### ETH/NNEO
 Good market creates a triangular arbitrage opportunity, but with USDC/NNEO which means not so much volume due to lack of liquidity.
 
 ### WBTC/BTCB
 Honestly this pair just has liquidity because of the pool weight and save heaven. Currently there is no good (triangular or cross exchange) arbitrage possible. We need more pairs with BTCB like BUSD/BTCB which would provide new triangular arbitrage opportunities with USDC/WBTC and USDC/BUSD.
 
 ### USDC/NEX
 Not bad at all, but only USDC/NEX is available at the moment. To expensive to do arbitrage in my opinion.
 
 ### ETH/BNB
 The forgotten child. No liqudity, no pool weight and no arbitrage opportunity. 
 
 ## Current Triangular Arbitrage Opportunities
 ### BUSD1
 + BUSD1-CEL1-USDC1-BUSD1
 + BUSD1-NNEO2-USDC1-BUSD1
 + BUSD1-SWTH-USDC1-BUSD1
 + BUSD1-USDC1-CEL1-BUSD1
 + BUSD1-USDC1-NNEO2-BUSD1
 + BUSD1-USDC1-SWTH-BUSD1
 ### CEL1
 + CEL1-BUSD1-USDC1-CEL1
 + CEL1-USDC1-BUSD1-CEL1
 ### BNB1
 None
 ### BTCB
 None
 ### ETH1
 + ETH1-NNEO2-USDC1-ETH1
 + ETH1-SWTH-USDC1-ETH1
 + ETH1-USDC1-NNEO2-ETH1
 + ETH1-USDC1-SWTH-ETH1
 + ETH1-USDC1-WBTC1-ETH1
 + ETH1-WBTC1-USDC1-ETH1
### NNEO2
 + NNEO2-BUSD1-USDC1-NNEO2
 + NNEO2-ETH1-USDC1-NNEO2
 + NNEO2-USDC1-BUSD1-NNEO2
 + NNEO2-USDC1-ETH1-NNEO2
### SWTH
 + SWTH-BUSD1-USDC1-SWTH
 + SWTH-ETH1-USDC1-SWTH
 + SWTH-USDC1-BUSD1-SWTH
 + SWTH-USDC1-ETH1-SWTH
### USDC1
 + USDC1-BUSD1-CEL1-USDC1
 + USDC1-BUSD1-NNEO2-USDC1
 + USDC1-BUSD1-SWTH-USDC1
 + USDC1-CEL1-BUSD1-USDC1
 + USDC1-ETH1-NNEO2-USDC1
 + USDC1-ETH1-SWTH-USDC1
 + USDC1-ETH1-WBTC1-USDC1
 + USDC1-NNEO2-BUSD1-USDC1
 + USDC1-NNEO2-ETH1-USDC1
 + USDC1-SWTH-BUSD1-USDC1
 + USDC1-SWTH-ETH1-USDC1
 + USDC1-WBTC1-ETH1-USDC1
### WBTC1
 + WBTC1-ETH1-USDC1-WBTC1
 + WBTC1-USDC1-ETH1-WBTC1
 
## New Markets
The following list represents pairs which could fill a gap and provide new opportunities.
### ETH/CEL
WTF why is this pair not on demex yet? 
### NEO/SWTH
Main market from switcheo exchange, I miss this market );
### BTC/SWTH
Either BTCB or WBTC both good desscions in my opinion. BTCB would be cheaper to trade.
### BUSD/BNB
This market could bring good volume too since Binance burns BNB on a regular basis.
 
