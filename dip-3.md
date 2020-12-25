---
yip: 3
title: Updating SP1 parameters
status: WIP
author(s): anon18382
discussions-to: https://discord.gg/2FaYk8VqT9
created: 12-25-2020
---
## Simple Summary
Update SP1 parameters to relax LP limits and increase rewards to incentivize DEBASE/DAI LPs to grow the DEBASE economy.

## Abstract
Since Pool 3 rewards in Degov halve tomorrow and there is a consensus that SP1 rewards are too low to incentivize LPs, this proposal calls to relax LP limits (both pool and wallet limits) and increase rewards to incentivize LPs during positive rebase cycles. While high inflation can cause downward price pressure, low inflation can lead to the same outcome since there is not enough incentive for LPs to take the Impermenant Loss and provide liquidity, which is very important for the protocol during positive rebase cycles. Inflation of some ideal range will grow the economy. The parameters suggested are a a best guess to create inflation within the ideal range.

## Motivation
LPs are an important part of the Debaseonomics protocol and incentivizing them is criticial for the growth of the DEBASE economy.
This proposal aims to incentivize LPs to provide liquidity during the positive rebase cycles using SP1.

## Technical specification

### Parameters to update
* rewardPercentage (Percentage of stabilizer pool rewards requested per reward duration) : Increase from 0.033 to 0.165 percent
* userLpLimit (LP limit per wallet): Increase from 3K to 6K
* poolLpLimit (Total LP limit per pool): Increase from 53k to 106k
