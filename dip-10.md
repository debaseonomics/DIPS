---
dip: 10
title: Automating rebase and funding past deployment costs
status: WIP
author(s): anon18382, @jusTaPunkk (@PunkUnknown)
discussions-to: https://discord.gg/2FaYk8VqT9
created: 02-10-2021
---
## Simple Summary
Proposal to automate rebases and to fund past code deployments. Rebasing is an important part of Debase stabilization. As gas fees climb, it's important that incentives remain for rebase to called. Likewise contract deployments costs need to be covered for deployment of new contracts, will be covered by builder's fees, but part of this allocation should be set aside for covering past contract deployments.
This proposal calls to set aside 0.5 pct of the Total supply for covering the cost of calling rebases in the future and for funding past deployment of contracts.
These Debases would be spent only during expasions to minimize price impact. 

## Motivation
To incentive rebase calling through automation, and to fund past contract deployments.

## Technical specification
All transactions will be moderated by VidarTheAuditor. Here are the addresses used to make contract deployments:

Deployer 1: 0x3c4dd566C5F9B441e59cBE4dA0822B81B9500afD (4.065 ETH in gas fees as per fees.wtf)

Deployer 2: 0x6dbbc75f2951B826730ac1b2B774C5dEC941A860 (3.172 ETH in gas fees as per fees.wtf)

Multisig executor 1: 0x610822D64Fe9e710F9Edc68144BE866db70109bd (0.674 ETH in gas fees as per fees.wtf)

Multisig executor 2: 0x38Ad8F7bbE670fb3384f7dFb06Ac3f44CEDB7b77 (0.877 ETH in gas fees as per fees.wtf)

Note: Funds would be spent only in expansion and all transactions will be mediated by VidarTheAuditor through the DEBASE multi-sig.
