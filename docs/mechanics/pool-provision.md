---
title: Pool Provision
parent: Mechanics
nav_order: 1
---

# Pool Provision

---

Pools serve two purposes

1. Allow TOKEN holders to DCA out on pumps rather than time, thereby limiting price impact (effectively volatiilty farming)
2. Lend out DAI so other token holders can unlock liquidity without selling
   
 Users single side deposit TOKEN, which adds to a shared pool in the range SPOT 2xSPOT, any buy pressure in is withdrawn as DAI, and the LP position repositioned again at spot.
   
In return for LPing, depositors get the following benefits

1.  Interest revenue generated when users borrow against the deposited TOKEN. This scales exponentially (when borrow demand is low, this is small as we don't need more LP, but when it's high, more goes to the LP to encourage more LPing) 
2.  All LP trading fees
3.  Ability to DCA out of their TOKEN position into DAI
4.  Most importantly, unlock greater borrow limits in the CDP markets on TOKEN

This mechanic has a subtle but important effect on the token market, by unlocking further borrow, and forcing LPers to only sell small amounts sustainably during price pumps, it moves the balance of buyers and sellers in the market. Less sellers, more net buyers, results in greater probability of sustained price pumps.

The risk Autonomous LPers take is negligible, it's the same as DCAing out of their position.