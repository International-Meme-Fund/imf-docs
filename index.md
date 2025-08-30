---
title: IMF User Manual
layout: default
nav_exclude: true
---

# IMF User Manual
{: .fs-9 }

The official International Meme Fund handbook.
{: .fs-6 .fw-300 }

[Launch app](https://app.imf.bz){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 target="_blank" }
[Connect with us](https://imf.bz){: .btn .fs-5 .mb-4 .mb-md-0 target="_blank" }

---

## IMF is a credit business built on Ethereum. 

International Meme Fund (IMF) offers lending markets for assets ignored by traditional DeFi. The IMF vault accepts **USDS** from lenders and issues loans to borrowers against volatile collateral.

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%;">
  <iframe 
    src="https://www.youtube.com/embed/U_E2jW9CrYI?si=YiK-xIMJ3GIan9t6&amp;controls=0" 
    title="YouTube video player"
    style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    allowfullscreen
    referrerpolicy="strict-origin-when-cross-origin">
  </iframe>
</div>

There is no DAO. There are no proposals. IMF is not governed...it is owned. **$IMF** is a takeover token, held accountable by the Salutary Standard. Whoever holds enough, controls it.

This is credit coordination for the chaos era.

**Taglines:**

- Loans for the longtail
- Crypto's lender of last resort
- Bank the unbankable

## How It Works

### Borrow

Use your tokens as collateral to borrow USDS. Each token has its own isolated market with its own loan-to-value (LTV) and oracle.

- **Collateral:** Supported tokens (eg. PEPE, MOG, SPX, JOE, REKT, CULT, BITCOIN, IMF, wstETH)
- **Loan Token:** USDS
- **Interest:** Paid to lenders
- **Liquidation threshold:** Liquidateable Loan-to-Value (eg. 77% LLTV) displayed per asset

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%;">
  <iframe 
    src="https://www.youtube-nocookie.com/embed/9rfCfP5frrA?si=RwjHb85pJwVLkNKG&amp;controls=0" 
    title="YouTube video player"
    style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    allowfullscreen
    referrerpolicy="strict-origin-when-cross-origin">
  </iframe>
</div>

**Steps:**

1. Deposit your collateral
2. Borrow USDS up to 50% LTV (frontend throttle)
3. Maintain a healthy position to avoid liquidation
4. Repay anytime to reclaim your collateral

**Interest Rates:**

IMF vaults use Morpho’s Adaptive Curve [Interest Rate Model](https://docs.morpho.org/learn/concepts/irm/){: target="_blank" }, which adjusts rates dynamically:

- Interest rises as utilization increases (above 90%)  
- Interest falls as utilization drops (below 90%)
- The model slowly adapts over time to keep target utilization near 90%  

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%;">
  <iframe 
    src="https://www.youtube-nocookie.com/embed/UJS6l8v2Zzo?si=O9CGBQggCIJYvp_Y&amp;controls=0" 
    title="YouTube video player"
    style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    allowfullscreen
    referrerpolicy="strict-origin-when-cross-origin">
  </iframe>
</div>

This keeps yield responsive and real.

**Liquidation Mechanics:**

Your position is protected by a **Safety Margin**:

- **Safety Margin of 0%** → your position is eligible for liquidation  
- A liquidator sells your collateral and repays your debt (for a small bonus)
- Rule of thumb for Safety Margin % is: `1 - ( LTV / LLTV ) * 100`

**Risks:**

- Price volatility
- Oracle failures
- Smart contract risk
- Liquidation in downturns

### Accelerate

Accelerate is a one-click leverage feature. You deposit a token, borrow USDS against it, and the protocol auto-buys more of the same token and re-deposits it as collateral. Net result: you're ~150% long at ~33% LTV (~57% safety margin for a 77% LLTV).

**Use cases:**

- Get more exposure without extra capital
- Stay long while unlocking extra liquidity

**Risks:**

- Liquidation due to over-leveraged exposure
- Swap slippage

### Amplify

Amplify turns idle tokens into productive assets without "selling." Deposit a single token, and IMF auto-deploys it into a **concentrated Uniswap v3 LP** against USDS.

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%;">
  <iframe 
    src="https://www.youtube.com/embed/xg6a7Q-KUwA?si=LPyP0fIbLpz3lzgs&amp;controls=0" 
    title="YouTube video player"
    style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    allowfullscreen
    referrerpolicy="strict-origin-when-cross-origin">
  </iframe>
</div>

**What happens:**

- LP fees earned from real trades
- USDS streamed out to fund the vault
- Profit takers become lenders

**Who it's for:**

* Treasuries and whales looking to earn without "selling"

**Risks:**

- Impermanent loss
- AMM volatility
- Contract risk

### Lend

Deposit USDS into the IMF vault and earn real yield from borrowers. Vault is built on [Morpho](https://docs.morpho.org/learn/concepts/vault/){: target="_blank" } with isolated markets per token.

**Details:**

- **Asset:** USDS
- **Counterparty:** Morpho vault
- **Interest source:** Borrowers
- **Performance fee:** 10% taken from borrower-paid interest

**Steps:**

1. Deposit USDS
2. Matched to borrowers via Morpho
3. Earn interest minus IMF’s cut
4. Withdraw anytime (subject to liquidity)

**Risks:**

- Smart contract
- Market & liquidation events
- Oracle feed problems

## Business Model

IMF earns revenue in multiple ways:

- **Performance Fees:** 10% of borrower-paid interest
- **Amplify Fees:** 0.01% on swaps routed through Amplify
- **Trading Fees:** 0.3% on IMF token trades
- **Yield:** Treasury earns ~10–20% from lending idle USDS
- **Market Gains:** Treasury goes long on select tokens
- **ETH Staking:** Treasury accumulates wstETH as collateral to loop borrow/lend spread

**Treasury** will also buyback $IMF to fund reward campaigns and support market making.

## $IMF Token

$IMF is not a governance token. It’s the first **legally enforceable on-chain takeover asset**, governed by the [Salutary Standard](https://www.salutary.io/){: target="_blank" }.

- **Control = Ownership**
- No voting. No proposals. No governance theater.
- Whoever owns a threshold amount (eg. 33%) owns IMF.

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%;">
  <iframe 
    src="https://www.youtube.com/embed/aX0wgApjKNQ?si=L8r90UysnyQNVLMd&amp;controls=0" 
    title="YouTube video player"
    style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    allowfullscreen
    referrerpolicy="strict-origin-when-cross-origin">
  </iframe>
</div>


### Tokenomics

 | Category | Share | Allocation | Description |
 |:---|:---|:---|:---|
 | Investors | 20.91% | 6,900,000 | Initial public presale distribution |
 | Treasury | 20.00% | 6,600,000 | Protocol growth and IMF ecosystem support |
 | Lenders | 20.00% | 6,600,000 | Rewards for lenders to bootstrap USDS lending |
 | Liquidity | 10.25% | 3,382,004 | Various liquidity positions deployed to AMMs |
 | Borrowers | 10.00% | 3,300,000 | Rewards for depositors to bootstrap USDS borrows |
 | Airdrops | 10.00% | 3,300,000 | Community contribution retroactive rewards |
 | [Team vesting](https://etherscan.io/token/0x05BE1d4c307C19450A6Fd7cE7307cE72a3829A60?a=0x2cde9919e81b20b4b33dd562a48a84b54c48f00c){: target="_blank" }  | 8.84% | 2,917,996 | Vesting plans managed via Hedgey finance |
 | ***TOTAL*** | ***100%*** | ***33,000,000*** | ***Maximum total supply (non-mintable)*** |

## Why IMF?

$IMF is not just exposure to the protocol. It *is* the protocol.

Owning $IMF means owning the infrastructure that underwrites millions in credit, captures real yield, and "governs" nothing, but controls everything.

<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%;">
  <iframe 
    src="https://www.youtube.com/embed/71W1LQyDRec?si=_jEkbSPZbsWlLl13&amp;controls=0" 
    title="YouTube video player"
    style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" 
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    allowfullscreen
    referrerpolicy="strict-origin-when-cross-origin">
  </iframe>
</div>

Here’s why IMF is worth taking over:

- **Built-in business model**  
  IMF earns revenue from *real borrowers* paying *real interest*. No inflation gimmicks, no mercenary yield farming. The protocol generates borrower-paid interest, swap fees, and LP yield.

- **Clear path to upside**  
  Protocol revenue flows to the Treasury. The Treasury buys back $IMF. Supply shrinks while protocol value grows. Owning $IMF today means owning a larger share of a more profitable machine tomorrow.

- **Underserved market with first-mover advantage**  
  Most tokens, especially memecoins, have zero access to credit. IMF lists them, collateralizes them, and absorbs their volatility. That’s not a bug, it’s the business model. As more tokens go live, and more degens borrow instead of sell, IMF becomes the backbone of the longtail.

- **Tokenholders capture it all**  
  Treasury, dealflow, and protocol fees flow to $IMF through market capture, buybacks, and accumulation. Just 33% of the token supply is enough to *own the machine.* Vaults, fees, LPs, and all.

- **Already live and working**  
  No roadmap hopium, no vaporware. IMF vaults are live, deployed on Morpho, supporting tokens like PEPE, MOG, JOE, SPX, IMF, REKT, BITCOIN, CULT and wstETH. As of August 2025, TVL exceeds $150M across 9 markets, with daily volume and real user flow. It’s not an idea, it’s operational.

- **Fully aligned with risk-takers**  
  There is no DAO, no bureaucratic committee, no governance theater. IMF is controlled by whoever takes the risk and accumulates the token. *Conviction is the mechanism.*

**In short:**  
$IMF is a high-conviction bet on a functioning credit protocol with real revenue, longtail market dominance, and takeover-enabled tokenomics.

The next wave of yield won’t come from ponzinomics. 

- It’ll come from credit.
- IMF is already underwriting it.
- **$IMF gives you the keys.**

## Next Steps

You’ve made it this far, which means you already see the bigger picture.

IMF is live, liquid, and lending. The vault is open. The token is trading. The play is underway.

Whether you’re looking to borrow, accelerate, amplify, lend, or accumulate ownership of the machine itself, the system is ready.

- [Connect with us](https://imf.bz){: target="_blank" }
- [Launch the app](https://app.imf.bz){: target="_blank" }
- [Buy $IMF](https://dexscreener.com/ethereum/0x59d813c1d0266278e2f5f146c0e222a6cfea83df){: target="_blank" }

Credit coordination for the chaos era.  
Let’s get to work.

## Contracts

### Tokens (Collateral)

- **MOG**: `0xaaeE1A9723aaDB7afA2810263653A34bA2C21C7a`
- **PEPE**: `0x6982508145454Ce325dDbE47a25d4ec3d2311933`
- **JOE**: `0x76e222b07C53D28b89b0bAc18602810Fc22B49A8`
- **IMF**: `0x05BE1d4c307C19450A6Fd7cE7307cE72a3829A60`
- **SPX**: `0xE0f63A424a4439cBE457D80E4f4b51aD25b2c56C`
- **REKT**: `0xdd3B11eF34cd511a2DA159034a05fcb94D806686`
- **BITCOIN**: `0x72e4f9F808C49A2a61dE9C5896298920Dc4EEEa9`
- **CULT**: `0x0000000000c5dc95539589fbD24BE07c6C14eCa4`
- **wstETH**: `0x7f39C581F595B53c5cb19bD0b3f8dA6c935E2Ca0`

### Credit (Lending)

- **USDS**: `0xdC035D45d973E3EC169d2276DDab16f1e407384F`
- More to come...

### IMF Token (Cross-Chain)

- **Ethereum mainnet**: `0x05BE1d4c307C19450A6Fd7cE7307cE72a3829A60`
- **Base L2 (bridge)**: `0x5C5B1DE218f86f00Fa547ac4f70DA2C39BB8A039`
- **Solana (bridge)**: `GgtzR8GGmK8iMHtV3nU6S9RaqWvDy7wpZECzMUXXkDT8`

### V2 Protocol (Active - Ethereum Mainnet)

- **Morpho Market**: `0xBBBBBbbBBb9cC5e90e3b3Af64bdAF62C37EEFFCb`
- **Morpho IRM**: `0x870aC11D48B15DB9a138Cf899d20F13F79Ba00BC`
- **IMF-USDS**: `0xdef1Fce2df6270Fdf7E1214343BeBbaB8583D43d`
- **MOG Oracle**: `0xa022aDB8C6bD4c25325A662cB928570a8e3966b4`
- **PEPE Oracle**: `0xad44b8257fb730e7344bcbe2908679324bd4dcf0`
- **JOE Oracle**: `0x8EE090A8486F40E059B61d23A9Ae9302508Acbbc`
- **IMF Oracle**: `0x82f0952DbB57d5a0b77Dc39A209D699a4584dFcd`
- **SPX Oracle**: `0x1913Bfde837324ef2e5B6b2A8017D7C661a538aB`
- **REKT Oracle**: `0x50ca523eEB5aED11C3A74F730dE82Aea9bD04d78`
- **BITCOIN Oracle**: `0xD131B09707A4a9D7Ce7c74D454d6Ae335e9955Fd`
- **CULT Oracle**: `0x851D005673a4BfD00B59eDe31424cD8BeB679CeF`
- **wstETH Oracle**: `0x871B119C40d512AD3839c7F15456d4717be8F12C`
- **Pump**: `0x2c17b87180ea16EaB0c67920F876AcE502d4316A`

### V1 Protocol (Deprecated)

- **MONEY token**: `0xb162caa6b63de33edc5d0a14b901fb6a54ee6b8f`
- **sbIMF token**: `0x3215c358b7a70c09e0a98827f744d107095e14e4`
- **PEPE/MONEY Uniswap v3 LP**: `0x210264fbcf553aa2e74a2c97e38aa1da237f30dd`
- **IMF/MONEY Uniswap v3 LP**: `0xe139cb8643897e28ad9dccf488151b6b55668ec2`
- **IMF Money Markets**: `0x30F75834cB406b7093208Fda7F689938aCBD1EeB`
- **Interest Rate Model (V1)**: `0xec39c6dF7947f2A4923d317B2805e41ed9116ecB`
- **PEPE/MONEY Oracle (V1)**: `0xB97b916436E4a3B0aEA6c6be2419c636D368035D`
- **MONEY/USD Oracle (V1)**: `0x66099a17C21a8dF6d949A704F484d544B81fdE1C`

### Security

- **Audit by Hashlock** ([@Hashlock_](https://x.com/Hashlock_){: target="_blank" })
- **Bug Bounty**: Hosted via Hashlock [bounty program](https://hashlock.com/bug-bounty/imf){: target="_blank" }