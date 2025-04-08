---
title: Morpho
parent: Integrations
nav_order: 2
---

# Morpho

IMF Borrow and Lend are built on [Morpho Blue](https://morpho.org){: target="_blank"}.
{: .fs-6 .fw-300 }

---

Morpho is the lending engine behind IMF’s credit system. A trustless framework for creating isolated, immutable lending markets for any token.

Each IMF market is deployed using Morpho’s [Multi-Market Factory](https://docs.morpho.org/overview/concepts/vault/){: target="_blank"}, with its own parameters, oracle, and risk model. No governance. No shared risk. No hidden switches.

## Why Morpho?

- Isolated markets prevent cross-asset contagion  
- Immutable contracts enforce predictable logic  
- [Dynamic interest rates](https://docs.morpho.org/overview/concepts/irm){: target="_blank"} based on real utilisation  
- Battle-tested with billions in TVL

Morpho lets IMF offer credit without compromise. **Transparent, modular, and built for the long tail of Ethereum**.

**Credit, without the complexity. Security, without the governance.**

## Market Parameters

### MOG-USDS

```
   martketID: "0x3f1d5c88c72432b04f2074499fe217468af49ddaa98bcb6ec80b08f76a82c6ec"
   Morpho: "0xBBBBBbbBBb9cC5e90e3b3Af64bdAF62C37EEFFCb"

   marketParams: {
       "collateralToken":"0xaaee1a9723aadb7afa2810263653a34ba2c21c7a",
       "irm":"0x870ac11d48b15db9a138cf899d20f13f79ba00bc",
       "lltv":"770000000000000000",
       "loanToken":"0xdc035d45d973e3ec169d2276ddab16f1e407384f",
       "oracle":"0xa022adb8c6bd4c25325a662cb928570a8e3966b4"
   }
   ```