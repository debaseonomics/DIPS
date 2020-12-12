---
yip: 1
title: Composing with Stabilizer-pool 1
status: WIP
author(s): anon18382, @jusTaPunkk (@PunkUnknown)
discussions-to: https://debaseonomics.medium.com/debase-v88-new-dawn-e6bc213796a3
created: 12-11-2020
---
## Simple Summary
Proposal to compose Stabilizer-pool 1 (SP1) with the Debaseonomics protocol, which will stabilize DEBASE, during positive rebase cycles.

## Abstract
SP1 will use a randomized threshold of positive rebases, to inflate part of the supply to the DEBASE/DAI LPs and stabilize the price of DEBASE during positive rebase cycles. Since the rewards are revoked when a non-negative rebase is hit, liquidity providers are incentivized to keep price above the upper limit of target range.  

## Motivation
DEBASE is supposed to stabilize towards the target range. In line with the vision of Debaseonomics to use stabilizer-pools to stabilize DEBASE price, SP1 will do so in expansion cycles (periods of high number of positive rebases, consecutive or otherwise). 

## Technical specification
SP1 will take in DAI/DEBASE LPs and provide rewards in DEBASE. 
The rewards are given out when n>= k positive rebases over a period of m rebase cycles occur, where k is sampled from a normal distribution with a known mean and standard deviation. 
The randomness incentivizes continous liquidity, as otherwise the rewards system can be manipulated if the blocktime of the rewards were known beforehand.
Furthermore, we use Chainlink VRF as a source of randomness given that on-chain randomness can be manipulated by miners.
The exact procedure to get the randomzied threshold is as follows: 
1. Preload an array of 100 integers, each of which is first sampled from a normal distribution of known Mean and SD. Once the array is provided, the integrity of the distribution can be estimated by governance. 
2. Have a counter that starts from zero and increments in value at every positive rebase. 
2. Use RNG at every rebase cycle, and mod the obtained randomn number with the size of array to pick one value from the array.
3. At every rebase cycle, check if integer obtained from 2. is >= the counter value.

### Configurable parameters

* Integer: Rewards requested by the the stabilizers
* Integer: Duration over which rewards will be distributed
* Boolean: Count positive rebases in sequence
* Boolean: Revoke further rewards in case of non-positive rebase
* Integer: Duration of rewards that will be revoked
* Boolean: Award rewards before previous rewards have been distributed
* Boolean: Pool is enabled for staking/withdrawal
* Normal distribution parameters
  * Integer[100]: Array filled with the numbers from Normal Distribution
  * Integer: Expected Value of the Normal Distribution (mean)
  * Integer: Stantard deviation of the Normal Distribution

### Additional information
Pool design by @PunkUnknown, with inputs from anon18382 on getting an approximation of Normal distribution on-chain
