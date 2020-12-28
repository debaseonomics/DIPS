---
yip: 4
title: Incentivize DEGOV/ETH LP
status: WIP
author(s): anon18382, @jusTaPunkk (@PunkUnknown)
discussions-to: https://discord.gg/2FaYk8VqT9
created: 12-28-2020
---
## Simple Summary
Proposal to incentivize DEGOV/ETH LPs with DEBASE rewards

## Abstract
Incentivize DEGOV/ETH pool with DEBASE rewards with the first incentive pool to reward rebase tokens correctly

## Technical specification
Since the rewards provided are in Debase, a rebasing token, a static reward rate in terms of the amount of tokens is conceptually incorrect 
(description of amount of rebasing tokens without reference to total supply is meaningless). Therefore, the LP rewards are calculated as a percentage of totaly supply instead. 

### Configurable parameters 
Note: Parameters are of type uint256 unless specified otherwise
* rewardPercentage: Rewards requested by the the pool as a percentage of the total supply
* duration: Duration over which rewards will be distributed
* userLpLimit: LP limit per wallet
* poolLpLimit: Total LP limit of pool

### Additional information
Pool design by @anon18382 & @PunkUnknown, built by @PunkUnknown
