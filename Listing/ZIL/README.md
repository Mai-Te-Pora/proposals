# Creation of ZIL related markets, pools and adjusting of the pool weight

Responsible for this proposal is Lynn Choy(Switcheo). She is assisted and advised by Coco and Devel(Validators).

Step 1 + 2 - Market Creation and Pool Linking will be proposed on chain right away since no one is effected in a negative way.

Step 3 - Pool Weight Adjustments requires further discussion and will be proposed in few days.

## New markets and pools (Step 1 + 2)

This proposal seeks to create the following markets:

- ZIL/BUSD
- ZWAP/BUSD
- GZIL/BUSD
- XSGD/BUSD

### ZIL-50-BUSD-50
ZIL is the main token of the Zilliqa ecosystem with. Pairing the Zilliqa assets with BUSD market marks the first on-chain USD stablecoin market for Zilliqa, and is a low-cost way to onboard Zilliqa users onto Demex.
Marketcap: >$1.2B

### ZWAP-50-BUSD-50
ZWAP is the governance token of ZilSwap and is the #4 token on the platform with over $19M in liquidity and a 24h trading volume of ~$300k.
Marketcap: $16M

### gZIL-50-BUSD-50
gZIL is the main governance token of Zilliqa. gZIL is currently the top-ranked token on ZilStream with the highest 24h volume, and ranked #2 in total liquidity on the platform. Similarly, pairing gZIL with BUSD will make it the first cross-chain pairing.  
Marketcap: ~$119m.

### XSGD-50-BUSD-50
XSGD is a stablecoin backed by the Singapore dollar, and exists in both ERC-20 and ZRC-2 token standards. XSGD is ranked 3rd on ZilStream with a 24h trading volume of ~$400k, and liquidity of $5.2M on ZilSwap. The XSGD-BUSD pair will also enable XSGD holders connection with the BSC ecosystem directly, for the first time.
Marketcap: $58M


## Pool Weight (Step 3)

For the ZIL/BUSD a pool weight of 5 points is planed in the beginning and will be adjusted in the next bigger round of pool weight adjustments like [TIP-17](https://forum.switcheo.foundation/topic/90/tip-16-extension-of-lp-rewards-updating-of-pool-weights)

The current pool system uses 95 points + optional 5 points for partnership promotions. Right now Locklet is granted this partnership promotion which will end in few days. Watch out for another forum post.

We want to continue the 100 point system, but due to the fact that the last change is less than one month old we suggest to increase the total number of pool weights to 105 + 5 partnership promotion.
This would mean that all pools will be reduced by the same relative ratio: ~9,09 %. For example if a pool has an ARP of 50% right now the new ARP would be 50% * (1-9.09%) = 45.45%.

| Pool      | Weight | APR     | New ARP*  |
|-----------|--------|---------|-----------|
| LKT/USDC  | 5      | 72.240% | 65.672%   |
| BUSD/NEO  | 11     | 64.456% | 58.596%   |
| BUSD/SWTH | 8      | 54.523  | 49.566%   |
| BTCB/BUSD | 6      | 46.269% | 42.063%   |
| BUSD/BNB  | 10     | 43.362% | 39.420%   |
| USDC/SWTH | 16     | 42.742% | 38.856%   |
| CEL/ETH   | 3      | 36.250% | 32.954%   |
| USDC/ETH  | 17     | 33.658% | 30.598%   |
| BNB/ETH   | 5      | 32.875% | 29.886%   |
| USDC/WBTC | 7      | 31.265% | 28.423%   |
| BUSD/CEL  | 4      | 29.814% | 27.104%   |
| NEO/ETH   | 4      | 28.884% | 26.258%   |
| WBTC/ETH  | 4      | 7.879%  | 7.163%    |
| ZIL/BUSD  | 5      | -       | 78.970%** |
| ZWAP/BUSD | 3      | -       | 47.380%** |
| gZIL/BUSD | 2      | -       | 31.590%** |
| XSGD/BUSD | 1      | -       | 15.790%** |

 .* Assuming the SWTH price and the total liquidity do not change.

** Based on the assumption of $100k liquidity and a SWTH price of $0.015.