---
Dip: 4
title: Single Sided Burn Mechanic For Governance
status: WIP
author(s): @Fabulousprizes
discussions-to: https://debaseonomics.medium.com/debase-v88-new-dawn-e6bc213796a3
created: 12-26-2020
---

## Simple Summary
Adopt a single sided burn of up to 100% in order to make governance deflationary and encourage long term staking

## Abstract
By using a single sided burn this creates a deflationary enviroment for long term stakers while punishing dumpers with either a progressive or fixed burn rate. You can also do a syatem where 100% of tokens are burned but you get a % of that in dai upon unstaking. So it's like a burn trade of sorts that can be a 90% burn 10% to governance/stakers.

## Motivation
To create a mechanism that rewards long term governance participation without direct incentivization that willl inevitably lead to inflation. I think this would further cement our position as a 'long term' stable coin.

## Technical specification
I thought to start off we would simply review what other protocols have done who are looking to create incentives for people to remain staked without increasing the rewards.

THUGS BUILT IN BURNING MECHANISM

$THUGS are burned when you send, sell, add and remove liquidity. The $THUGS burn rate adjusts depending upon $THUGS price. The lower the price the higher the burn rate, vice versa. The maximum burn is 50% and the minimum is 0.5%. There is no way around this and your tokens will be burned based on the calculated burn rate.

Here's how the burn rate is calculated:
Burn rate = 50% / (Current $THUGS price /  $0.36760313)

For example, with a current $THUGS price = $2.297519562,
Burn rate = 50% / ($2.297519562 / $0.36760313)
                = 8%

Narwhal Token is another BNB protocol that takes a similar but less harsh approach to burns and also has a way of using spreads for auto-dividends.

Contract address (Burn) is here.

These burnt $THUGS are split into the following allocation, with 51% going to a burn address and the other 49% going to a Thugs.Fi vault, whcih is called a protection fund. Tokens in this protection fund are used for future development, marketing, business relations, Liquidity Provider Air Drops, community management, community contests, THUGS DAO payments and various other expenses.

How the NAR token's 5% burn works.

When a user transfers NAR token, that is when calling the transfer interface and transferFrom interface of the smart contract, 5% trading fees will be deducted, 2.5% of it will be directly destroyed, the remaining 2.5% will be transferred to the dividend pool.

The idea would be to apply something like this to a Degov Staking pool thus creating a major incentive for people to stake long term or at least until they had recouped the burn. Another mechanism I've seen prove to be effective is the 'ape trap' employed by surf. Basically they lured people in with short but super juicy rewards but they had a 20% unstaking fee. Then when rewards were cut people would unstake for high yields benefitting those who were there for the long run. Duck Dao has a similar approach to this where they alter reward distributions where one week it will be high the next week low. The premise being when you combine that with a burn it creates a situation where if you try to stake for the high apy and unstake for the low you will lose money. But often they will make it where people will be down roughly 5% if they unstake after the high apy period with burn. You would be surprised how many people continually unstake at a loss after high apy ends to chase after some next higher apy only to come back the next week literally.

Duck Dao also does regular snapshop and NFT rewards that are done randomly the result is that unless you are staked long term you are never going to stake just in time to get them. They also do stuff like release all their market maker rewards at once creating a day where APY becomes insane for short period of time. This puts them on top of all the degen leaderboards and if you talk to defiyield.info you can probably get on his daily chart whenever you do this too. 

I also thought it might be helpful to have a zerion/apy vision type thing where you can visually see your gains in LP with big green numbers when you log in. Not only that I think showing people rewards vs LP value might be very helpful. Beacause I think many people are thinking you are being diluted 75% if it goes from 8$ to 2$ which simply isn't the case at all. I also think it might be worthwhile for us to do an incubation with DuckDao which could provide us with much needed long term liquidity. Basically after incubation they offer liquidity at a 'fixed fee' which could be good for us. Because it might be worth spending some governance money on liquidity to maintain stabiltiy should a large whale ever unstake or malcious actors attempts to intentionally destabilize the protocol. 

https://duckdao.io/apply/

https://thefoundry.one/

I also think we would seriously benefit from being added to zapper.fi or by adding an 'ape' button for usdt/eth on our main page where you can buy in with one click and using USDT allows some cross-chain implenetation. I am not sure exactly how it works but I know N3rds is doing something like this. 

The last form of burn I will go over is unilateral one sided burn this is what duck dao uses and it's where all of one side of the LP is burned upon unstaking allowing you to have total control over supply. This deflationary mechanism rewards users that remain liquidity providers for the longest period of time. 

The other things they are using are 'peak weeks' multipliers and NFT distribution to stakers to incentivize people to stick around for the long term. Some of these things are definitely gimmicks if you ask me but they work. They've also done a partnership with Ivan on Tech and another Tech youtuber. This is huge because it brings in the 'normie' crowd of people who might otherwise never invest in something like this. But having someone explain to them why this is actually way less risky than whatever they're currently into would be really helpful I think. Because I have had to realize recently that most people aren't gonna read the medium. If you don't like this idea I was thinking an infographic might be helpful. Basically a picture that explains Debase in as few words as possible and using pictures to illustrate concepts. Because most people don't like reading and simply would rather avoid it if possible. To them Crypto is a leisure activity which is why they are reluctant to read or do anything that might be taxing.

I think that debase has really strong fundamentals thus I think we need to work on the gimmicky/marketing side of things a bit more. Because it's clear to me that anyone who knows can see that debase is far superior to these other 'algo coins'. I think winning over an influential twitter personality who normally hates these projects such as @degenspartan or someone like that could be a big win. Honestly we need to create some kind of incentivized marketing team, where we set marketing bounties such as 'get a crypto influencer to tweet about debase' we could even make the rewards 'exclusive nfts' which will have 'further implentation down the line' which is 'a secret for now'. 

I personally love the debase NFTs and have stayed up many a nights trying to hit the rebase button to win one. If I was somehow able to win one thro LP providing I would literally never unstake until I got the one's I wanted. Because I am emotional an irrational like most people. You can also allow for wrapping of NFTs to provide liquidity on them and the NFTs themselves can be backed with Debase LP or eth etc. Giving them 'intrinsic' value as well as extrinsic, we could even have NFTs that were synthetic debase derivatives of somekind.

I apologize for going on a bit of a tangent at the end here, let me know if there's anything here I should look into more or any competitors you think I should be researching.
