---
dip: 10
title: Decrease rebase lag for expansions
status: WIP
author(s): punkUnknown
discussions-to: https://discord.gg/2FaYk8VqT9
created: 12th February 2021
---
## Simple Summary
Proposal to decrease rebase lag when debase going into expansion cycles. To help boost debase market cap.

## Motivation
Every time debase is above it's peg and a supply expansion happens. Debase's supply expands in relation to how far debase is away from it's peg in order to induce a user's to sell newly earned debase. But to control these supply expansions so debase doesn't suffer supply shocks, expansion are reduced by a rebase lag parameter. Currently expansions are reduced by dividing the new supply expansion by 30. These is very high and to increase debase's expansion it needs to be reduced.

### Parameters to update
* Rebase lag should be set to 25,20,15,10