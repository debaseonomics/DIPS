---
dip: 5
title: Debased MPH pool (DM88)
status: WIP
author(s):  @McFly, @ZeframLou, @anon18382, @jusTaPunkk (@PunkUnknown)
discussions-to: N/A (Suprise launch)
created: 01-07-2020
---
## Simple Summary
Create pool (DM88) that locks-up Debase-Dai LPs for yield in DAI, MPH and Debase rewards to be released at time of unlock. Debaseonomics governance collects a fee for creating the strategy and saving user's gas fees through collective staking.

## Abstract
Create pool that locks-up Debase-Dai LPs for 30 days for yield in DAI, MPH and Debase rewards to be released at time of unlock. Debaseonomics governance collects a fee for creating the strategy and saving user's gas fees through collective staking.

## Motivation
[88mph](https://88mph.app/) sits on the Debaseonomics governance to purse mutual goals. To this end, this pool DM88 will increase liquidty in the Debase/Dai pair which is important for an algorthmic stablecoin especially during expansion. It also increases the Total Value Locked in 88mph to create the right synergy between the 2 protocols. The more TVL on 88mph, the better Debase-Dai LPs' yield will be.

## Technical specification
DM88 pool will lock Debase-Dai LPs for 30 days. The provided LP is unstaked by contract, with the DAI component being used in the 88mph fixed-interest rate pool. 
The linearly vested MPH rewards are staked in the 88mph's staking pool to earn staking rewards coming from 88mph protocol fees, and yield-farmed tokens earned on the underlying money markets used by 88mph. The MPH is staked collectively, rather than induvidually saving on gas fees.
Finally at the end of the LP depositor's lock period, the percentage of the MPH to be returned to the fixed-interest rate pool is paid back as per conditions of the deposit. The DAI + DEBASE originally in the LP is returned back to the LP depositor, along with the DAI fixed yield, MPH rewards, MPH staking rewards, and Debase rewards. A fee is taken by the Debase treasury as percentage of the DAI yield+MPH rewards+MPH staking rewards.
Review here for a visual representation: [https://cutt.ly/OjgN7iM](https://cutt.ly/OjgN7iM)

### Configurable parameters 
Note: Parameters are of type uint256 unless specified otherwise
*poolLPlimit: Total LP limit of Pool
*walletLPlimit: Max deposit per wallet
*plimitEnabled(Boolean):Is total lp limit enabled 
*wlimitEnabled(Boolean): Is Max Deposit per wallet enabled 
*rewardRate: Percentage of total supply of Debase awarded per LP
*fee: Percentage of fee taken by treasury from the DAI yield+protocol fees and MPH rewards
