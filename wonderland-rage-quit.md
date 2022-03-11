<h1><p align=center>Wonderland Rage Quit</h1>

Written by [@fbsloXBT](https://twitter.com/fbsloxbt), March 10th, 2022

---

<h3>Introduction:</h3>

Wonderland is OHM fork, originally founded by @danielesesta, based on Avalanche blockchain. During OHM fork season in Q3-Q4 of 2021, has amassed a large treasury, but due to different circumstances (both general decline of OHM forks, and discovery that co-founder and treasury manager @0xSifu is actually QuadrigaCX-related developer and ex-convict Michael Patryn), the token value plummeted and at the time of writing (March 9th, 2022), wMEMO token (wMEMO is a wrapped version of MEMO, staked version of TIME. It's not increasing in amount, only in value (against MEMO)) is trading at $26,544.

Governance proposal was passed that will allow users to exchange their wMEMO for MIM at backing price - Rage Quit: https://www.wonderlandforum.xyz/t/wip-5-offer-a-rage-quit-option-to-wmemo-holders/

Treasury is located at following addresses: [zapper link](https://zapper.fi/bundle/0xb6b80f4ea8fb4117928d3c819e8ac6f1a3837baf,0x355d72fb52ad4591b2066e43e89a7a38cf5cb341,0x1c46450211cb2646cc1da3c5242422967ed9e04c,0x78a9e536ebda08b5b9edbe5785c9d1d50fa3278c):
* 0xb6b80f4ea8fb4117928d3c819e8ac6f1a3837baf
* 0x355d72fb52ad4591b2066e43e89a7a38cf5cb341 
* 0x1c46450211cb2646cc1da3c5242422967ed9e04c 
* 0x78a9e536ebda08b5b9edbe5785c9d1d50fa3278c

The total value of treasury is $698,846,866 as per Zapper.com bundle listed above (we will get back to calculating actual backing shortly).

Since TIME/MEMO/wMEMO tokens are backed by the treasury and are trading below their intrinsic value, there was a "Rage Quit" proposal created, proposing to allow anyone to exchange their wMEMO for underlying MIM (stablecoin) tokens. [Proposal](https://snapshot.org/#/bestfork.eth/proposal/0xf140cd15c8c9803dc698e907c50837b97d967c1b716661de3573c2f7ba410e2d) has passed with 95.79% votes for.

---

<h3>Treasury:</h3>

If we want to arbitrage the difference between wMEMO market price and wMEMO rage quit price, we first need to get the correct worth of the treasury (excluding wMEMO and illiquid assets). Treasury addresses are listed above. Here is a breakdown by networks that treasury holds assets on:

| AVAX | ETH| FTM|
| ----------- | ----------- | ----------- |
| 35,600,000 MIM| 48,246,542 UST |6,607,000 MIM|
| 8,370 WETH| 22,804,959 USDT |2,403,860 FTM|
|82,031,115 MIM (in Sushi MIM-WAVAX LP)|20,300,000 USDC ||
|1,112,921 WAVAX (in Sushi MIM-WAVAX LP)|19,727,822 MIM||
|18,552,736 MIM (in Sushi MIM-wMEMO LP)|815,103 CVX ||
||3,994 WETH||
||92.15 WBTC||
||1,063,829 SUSHI ||
||8626.5 ETH (in UNI-v3 MIN-ETH LP)||
||1667.6155 ETH (in Sushi BSGG-ETH LP)||
||1,095,076,090 SPELL (staked)||
||10,150 CVX (claimable)||
||67,705 CRV (claimable)||

Sum:

MIM: 162,518,673 ~ $162,518,673

WAVAX: 1,112,921 ~ $82,022,277

WETH: 22,658 ~ $56,418,420

UST: 48,246,542 ~ $48,246,542

USDT: 22,804,959 ~ $22,804,959

USDC: 20,300,000 ~ $20,300,000

CVX: 825,253 ~ $13,220,553

SPELL: 1,095,076,090 ~ $4,187,570

WBTC: 92.15 ~ $3,595,378

FTM: 2,403,860 ~ $3,245,211

SUSHI: 1,063,829 ~ $3,170,210

CRV: 67,705 ~ $140,149

<h4>Total: $419,869,942</h4>

Amount of wMEMO that can rage quit is 12,060 wMEMO (of which only ~6k are whitelisted to rage quit).

$419,869,942 / 12,060 = ***$34,815***

Current price: $26,500, difference: ***31.3%*** 

---

<h3>Risks:</h3>

***High risk:*** The biggest risk is caused by the centralization of Wonderland treasury. Funds are not managed by autonomous smart contracts but are instead held in a 2/3 multi-signature wallets. Only one wallet has an ENS name, `token🐳.eth : 0x8a7f7c5b556b1298a74c0e89df46eba117a2f6c1`. 
***It is completely up to them to decide if they will honor the governance proposal.***

***Low risk:*** Another risk is MIM de-peg. Currently, the treasury holds 162M MIM tokens, and liquidity on Curve is low (82% of the 1.2B pool is in MIM, only 17% in 3CRV (DAI, USDC, USDT)). But less than 6k wMEMO has whitelisted for rage quit, so in the worst-case scenario, 81M MIM will be sold, which would not move the peg (even full 162M would not be enough to move the price).

---

<h3>Trade execution:</h3>

Many exact details (like rage quit contract, if we will be only able to exchange the amount held at the time of whitelist snapshot) are not yet available, I don't think there are many logistical issues for trades below 8 figures, there is decent wMEMO liquidity on Sushiswap ($38M at the time of writing), simply buy wMEMO, wait for RQ and exchange it for MIM, which you can then swap for other stablecoins on Curve.

Even if you are not whitelisted, Abracadabra.money recently [passed](https://snapshot.org/#/abracadabrabymerlinthemagician.eth/proposal/0xb86da61c44c6e91f94736994144fbb7a757694f403279eadd93572112dfc0cc3) a [Expecto Patronum proposal](https://forum.abracadabra.money/t/aip-7-expecto-patronum-a-shield-for-all-frogs/2755), which allows them to purchase 30B SPELL worth of wMEMO. At the moment, that is $100M+ with of SPELL, so liquidity should not be a problem. The bigger issue is 72h lockup period before users will receive their SPELL. But luckily, SPELL-PERP futures are available on [FTX](https://ftx.com/referrals#a=fbsloXBT), so you can hedge your exposure during this time.

---

<h1><p align=center>DISCLAIMER</h1>

<h3>Do Your Own Research</h3>

My (@fbslo/@fbsloXBT) content is intended to be used and must be used for information and education purposes only. It is very important to do your own analysis before making any investment based on your own personal circumstances.

---

<h3>No Investment Advice</h3>

I (@fbslo/@fbsloXBT) am not a broker/dealer, I am not an investment advisor, I have no access to non-public information about this project, and this is not a place for the giving or receiving of financial advice, advice concerning investment decisions or tax or legal advice. I am not regulated by the Financial Services Authority.

No content on the site constitutes - or should be understood as constituting - a recommendation to enter in any transaction or to engage in any of the investment strategies presented in this content.

<h3>No Reliance</h3> 

Accordingly, I will not be liable, whether in contract, tort (including negligence) or otherwise, in respect of any damage, expense or other loss you may suffer arising out of such information or any reliance you may place upon such information.

<h3>Investment Warnings</h3> 

We would like to draw your attention to the following important investment warnings.

-   The value of investments and the income derived from them can go down as well as up.
-   Investors may not get back the amount they invested - losing one's shirt is a real risk.
-   Past performance is not a guide to future performance.
