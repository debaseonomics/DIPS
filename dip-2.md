---
yip: 2
title: Updating SP1 parameters
status: WIP
author(s): anon18382
discussions-to: https://discord.gg/2FaYk8VqT9
created: 12-17-2020
---
## Simple Summary
Update SP1 parameters to relax LP limits and increase rewards to incentivize DEBASE/DAI LPs.

## Abstract
Since SP1 has been launched and the LP limit was hit much faster than expected, this proposal calls to relax LP limits (both pool and wallet limits) and increase rewards to incentivize LPs during positive rebase cycles.

## Motivation
LPs are an important part of the Debaseonomics protocol and incentivizing them is criticial for the growth of the DEBASE economy.
This proposal aims to incentivize LPs to provide liquidity during the positive rebase cycles using SP1.

## Technical specification

### Parameters to update
* rewardPercentage (Percentage of stabilizer pool rewards requested per reward duration) : Increase from 0.0055 to 0.033 percent
* userLpLimit (LP limit per wallet): Increase from 1K to 3K
* poolLpLimit (Total LP limit per pool): Increase from 30k to 53k
