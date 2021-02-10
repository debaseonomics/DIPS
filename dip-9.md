---
dip: 9
title: Composing with Stabilizer-pool 2
status: WIP
author(s): anon18382
discussions-to: https://discord.gg/2FaYk8VqT9
created: 9th Feburary 2021
---
## Simple Summary
Proposal to compose Stabilizer-pool 2 (SP2) with the Debaseonomics protocol, which will stabilize DEBASE, during negative rebase cycles.

## Abstract
SP2 will use an new seigniorage system that seeks to minimize time price is far from peg thus overcoming one of the main issues of current seignoirage systems.

## Motivation
DEBASE is supposed to stabilize towards the target range. In line with the vision of Debaseonomics to use stabilizer-pools to stabilize DEBASE price, SP2 will do so in contraction cycles through an seignoirage system.

## Technical specification
Details of the system can be found here:
https://debaseonomics.medium.com/sp2-user-guide-shut-the-door-behind-you-369646ed72

### Configurable parameters 
A complete list of parameters and their values is available here: 
https://thegraph.com/explorer/subgraph/debaseonomics/burnpool?version=current

The most pertinent ones are listed below:

Cycle length (Duration over which rewards are given out in expansion): 5 Epochs

Epoch time: 6400 Block (~24 days)

Oracle block Period (TWAP oracle for coupon window): 1000 Blocks (~4 hrs)

Builders fee (request made to rewards contract as a percentage of the cycle's reward pot): 20% (upto 5% shared with community)

### Additional information
Pool design by @Punkunkown, @anon18382 and Sabretooth
