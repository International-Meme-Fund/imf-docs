---
title: Pooling
parent: Mechanics
nav_order: 1
---

# Pooling: A Better Way of Providing Liquidity

---

Our pooling feature is designed as a superior form liquidity provision. Users not only can earn LP fees while gradually DCA'ing out of their positions, ensuring a structured and sustainable exit, but the extracted stablecoins are pulled directly from the LP, preventing losses due to market downturns. Additionally, these **DCA'd stablecoins are immediately deployed into high-yield lending,** maximizing capital efficiency.

Liquidity pools in the protocol serve two primary functions:

1.  **Facilitating managed exits for TOKEN holders** -- Holders can gradually **dollar-cost average (DCA) out of their position** in a structured liquidity provision (LP) model.
2.  **Providing high-yield lending opportunities** -- The DAI extracted from the DCA process is lent to borrowers at competitive interest rates.

## Mechanics of Liquidity Provision

Users **single-sided deposit TOKEN** into a shared liquidity pool. This pool operates within a price range of **SPOT to 2x SPOT.** Periodically, a portion of the pool's buy pressure is converted into DAI, while the LP position is **rebalanced to the current spot price.**

## Benefits for Liquidity Providers

Liquidity providers (LPs) receive several key advantages:

-   **Interest revenue from borrowers:** As users borrow against the deposited TOKEN, LPs earn interest. This revenue scales **exponentially** with borrowing demand---when demand is low, minimal incentives are needed, but when demand increases, higher rewards attract additional liquidity.
-   **Trading fees from liquidity provision:** LPs earn a share of trading fees generated within the pool.
-   **Automatic DCA into DAI:** LPs can gradually **convert their TOKEN holdings into DAI** without causing abrupt market impacts.
-   **Enhanced borrowing limits:** By participating as LPs, users can **unlock higher borrowing limits** within the collateralized debt position (CDP) markets for TOKEN.

## Market Impact

This mechanism has a **subtle but significant effect** on TOKEN's market dynamics. By unlocking additional borrowing capacity and ensuring that liquidity providers **only sell in a controlled manner during price increases,** the system **reduces overall selling pressure while increasing net buying activity.** This increases the probability of **sustained price appreciation.**

## Risk Considerations

The risk to **autonomous LPs** is minimal, as the process mirrors **a structured DCA strategy.** LPs systematically reduce their TOKEN holdings over time while benefiting from yield and increased borrow demand, ensuring sustainable liquidity management.