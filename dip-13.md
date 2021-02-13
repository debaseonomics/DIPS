---
dip: 13
title: Remove randomness from SP1 and increase it's rewards
status: WIP
author(s): punkUnknown
discussions-to: https://discord.gg/2FaYk8VqT9
created: 12th February 2021
---
## Simple Summary
Proposal to remove randomness from stabilizer pool 1 and to remove it's rebase counter and replacing it by a pool that gives rewards during rebase expansions/stability and pauses rewards during contraction. Due to rising gas costs and the continued price appreciation of LINK, it would be increasingly expensive to maintain the LINK powered random number generator in SP1. 
Removing randomization also simplifies the rewards scheme and encourages liquidity. Rewards are given out as soon as a positive rebase happens and pauses rewards as soon as a negative rebase happens. The positive and negative rebases have different reward rates. 

## Motivation
Simplification of the pool and higher APRs will increase interest in the pool and lower gas costs to run the pool.

This proposal also proposes increasing reward requests by the stabilizer pool. So we can increase the pool's apy and hence bring more liquidity back to debase

## Technical specification

1. SP1 gives out continous rewards over a period of 1 month. 
2. Rewards stop when Debase TWAP price falls below < 0.95 $Dai
3. Rewards start when Debase TWAP price goes above > 0.95 $Dai
4. Increasing rebase reward to 0.005 during positive rebases and 0.0025 during stability (180000 and 90000 Debase per month at current Total supply respectively)
5. Builders fee is 20 pct (requested seperately from rewards contract)
