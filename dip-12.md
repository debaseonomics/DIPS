---
dip: 10
title: Decrease rebase lag for expansions
status: WIP
author(s): punkUnknown
discussions-to: https://discord.gg/2FaYk8VqT9
created: 12th February 2021
---
## Simple Summary
Every time DEBASE is above it's peg and a supply expansion happens, DEBASE's supply expands in relation to how far epoch price of DEBASE is from stability range, in order to induce an user to sell newly earned DEBASE. But to control these supply expansions so debase doesn't suffer supply shocks, expansion are reduced by a rebase lag parameter. Currently expansions are reduced by dividing the new supply expansion by 30. Reducing it should be considered to boost reflexivity.

## Motivation
Proposal to decrease rebase lag when debase going into expansion cycles to boost reflexivity. 

## Technical specification
The change will be mediated by VidarTheAuditor through the DEBASE multi-sig.
### Parameters to update
* Rebase lag when epoch price > 1.05 DAI: Choices are 10, 15, 20, 25
