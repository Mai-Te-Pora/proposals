# Creation of ZIL related markets, pools and adjusting of the pool weight

## New markets and pools
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


## Pool Weight

For the ZIL/BUSD a pool weight of 5 points is planed in the beginning and will be adjusted in the next bigger round of pool weight adjustments like  (TIP-16)[]

The current pool system uses 95 points + optional 5 points for partnership promotions. Right now Locklet is granted this partnership promotion which will end in few days. Watch out for another forum post.

I want to continue the 100 point system, but due to the fact that the last change is less than one month old I suggest to increase the total number of pool weights to 100 + 5 partnership promotion.
This would mean that all pools will be reduced by the same relative ratio: 4.76 %. This means if a pool has an ARP of 50% right now the new ARP would be 50% * (1-4.76%) = 47,61%.

