---
dip: 13
title: Remove randomness from SP1 and increase it's rewards
status: WIP
author(s): punkUnknown
discussions-to: https://discord.gg/2FaYk8VqT9
created: 12th February 2021
---
## Simple Summary
Proposal to remove randomness from stabilizer pool 1 and to remove it's rebase counter. Replacing it by a pool that gives rewards during rebase expansions and pauses rewards during contractions.

## Motivation
Due to rising gas costs and bull market in the crypto sphere. It has been very expensive to maintain the link powered random number generator for pervious versions of stabilizer pool 1. Along with this due to the randomness itself interest in the stabilizer pool has been less than stellar. 

So by removing randomization from sp1 and replacing it with a system that promises a stable reward scheme. Where rewards are given out as soon as a positive/neutral rebase happens and pausing rewards as soon as a negative rebase happens. Will increase interest in the pool and lower gas costs to run the pool.

This proposal also proposes increasing reward requests by the stabilizer pool. So we can increase the pool's apy and hence bring more liquidity back to debase

## Technical specification

1. SP1 gives out continuos rewards over a period of 1 month. 
2. Rewards stop when Debase TWAP price falls below < 0.95 $Dai
3. Rewards start when Debase TWAP price goes above > 0.95 $Dai
4. Increasing rebase reward from 0.0002 to 0.005 (180000 Debase per month)
