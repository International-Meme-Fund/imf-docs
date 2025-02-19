---
title: CDPs
parent: Mechanics
nav_order: 2
---

# Collateralized Debt Positions

---

At its core, our system is similar to OG Aave, users put up assets as collateral and borrow against them. Each borrow receives DAI, and each repay returns it to our Morpho multi-market. As such the system both scales and unwinds gracefully based on the current mark to market of the collateral backing our DAI.

In order for a TOKEN to unlock a borrow market, the community needs a pool of 69k USD equivilant. This is for the social signal that the community wants to unlock borrow.  

Once a token hits the pool minimum, the protocol will turn on a DIA oracle (assuming DIA's oracle criteria are met), and create a new morpho market for the pair TOKEN/DAI. On launch, the IMF will pay for all oracle gas fees, with the aim to protocolise this in the future.

Borrow limits are adjusted as on chain liquidity changes. A great property of this approach is we can keep collaterisation ratios constant, as the risk in the system is managed by scaling up total borrow with liquidity.

The interest rate is priced on a compound style curve. As a TOKEN community manages to shift sell demand to borrow, the interest rate rises. This will naturally attract yield chasers to deposit their DAI into the multi-market, or more TOKEN holders into the pool. Put another way, the market will find a natural equilibrium between borrow demand and the fair market interest rate.

It's worth noting that high interest rates in the short term have a negligable impact on holders profit, but have an outsized impact on TOKEN price. 

TODO: moon math calculator embed.