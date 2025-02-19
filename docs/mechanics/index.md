---
title: Mechanics
nav_order: 3
---

# Mechanics

Two core components work together to allow provision of stablecoins.
{: .fs-6 .fw-300 }

---

Both of these work together to allow us to provide collateralized debt:

- Pool provision, which creates a managed UniV3 LP position between TOKEN and DAI
- Collateralised Debt Module, which allows borrow of DAI using TOKEN as collateral

The managed LP farms volatility. The Farmed DAI is lent out for other TOKEN holders to borrow against

TODO: Flywheel image