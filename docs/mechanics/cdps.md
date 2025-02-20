---
title: CDPs
parent: Mechanics
nav_order: 2
---

# Collateralized Debt Positions

---

The debt component of our CDP operates similarly to other CDP platforms, like Aave, where users deposit assets as collateral to borrow against them. Each borrowing event results in the issuance of DAI, while repayments return DAI to our Morpho multi-market. This design ensures that the system scales and unwinds efficiently based on the mark-to-market valuation of the collateral backing the issued DAI.

## Unlocking a Borrow Market

To enable borrowing for a specific token (TOKEN), the community must establish a liquidity pool with a minimum equivalent of **$420,000 USD.** This threshold serves as a social signal, indicating sufficient interest and demand for the token's borrowing functionality.

Once the liquidity requirement is met, the protocol will activate a **DIA oracle** (provided that DIA's oracle criteria are satisfied) and create a new **Morpho market** for the **TOKEN/DAI** pair. Initially, the **IMF** (International Meme Fund) will cover all oracle gas fees, with the long-term goal of transitioning this responsibility to the protocol.

## Borrow Limits and Liquidity Adjustments

Borrowing limits are dynamically adjusted based on on-chain liquidity. A key advantage of this approach is the ability to maintain stable collateralization ratios, as the system mitigates risk by scaling borrowing capacity in proportion to available liquidity.

## Interest Rate Mechanism

Interest rates follow a **Compound-style** curve. As the TOKEN community shifts sell pressure towards borrowing demand, the interest rate increases accordingly. This rise in rates incentivizes:

-   **Yield-seeking lenders** to deposit additional DAI into the multi-market.
-   **TOKEN holders** to contribute more liquidity to the pool.

This mechanism naturally drives the market toward an equilibrium between borrowing demand and a fair market interest rate.

It is important to note that **short-term spikes in interest rates have a negligible impact on overall holder profitability** but can have a **significant effect on the price of TOKEN** due to increased borrowing demand.