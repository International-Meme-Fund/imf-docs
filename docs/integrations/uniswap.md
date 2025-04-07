---
title: Uniswap
parent: Integrations
nav_order: 1
---

# Uniswap

IMF uses [Uniswap v3](https://docs.uniswap.org/contracts/v3/overview){: target="_blank"} to power its Pools.
{: .fs-6 .fw-300 }

---

Rather than creating a custom liquidity layer, IMF plugs directly into Uniswap, the most trusted AMM in DeFi, and optimises it for credit provisioning.

This means IMF doesn’t need to build liquidity from scratch. Instead, it builds on Uniswap’s deep ecosystem, robust infrastructure, and proven economic design.

### Why Uniswap?

- Concentrated liquidity improves LP efficiency  
- Battle-tested infrastructure trusted with billions  
- Permissionless and composable with every major DeFi protocol

IMF configures each Pool as a single-sided token deposit, paired with [USDS](https://sky.money){: target="_blank"}, and deployed into a protocol-optimised Uniswap v3 position. Users don’t manage LP strategy. The protocol does it for them.

**This integration gives tokens real liquidity, and makes that liquidity productive.**