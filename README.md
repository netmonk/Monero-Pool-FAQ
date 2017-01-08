# monero-pool-faq
<!-- vim-markdown-toc GFM -->
* [General purpose of this document](#general-purpose-of-this-document)
* [Questions and Answers](#questions-and-answers)
    * [I mine since few time, but my balance is still zero](#i-mine-since-few-time-but-my-balance-is-still-zero)
    * [when I will get my monero ?](#when-i-will-get-my-monero-)
    * [Can I get paid on market wallet directly ?](#can-i-get-paid-on-market-wallet-directly-)
    * [How can I check if the balance is updated?](#how-can-i-check-if-the-balance-is-updated)
    * [why do so many monero pool sites have very similar layout is their an open source git or something?](#why-do-so-many-monero-pool-sites-have-very-similar-layout-is-their-an-open-source-git-or-something)
    * [hy can someone help me? My account is showing transfer founds but nothing is showing up in my wallet?](#hy-can-someone-help-me-my-account-is-showing-transfer-founds-but-nothing-is-showing-up-in-my-wallet)
    * [What graphics card are you using?](#what-graphics-card-are-you-using)
    * [Wolf0 are you the famous miner developper ?](#wolf0-are-you-the-famous-miner-developper-)

<!-- vim-markdown-toc -->


## General purpose of this document

Monero is a new generation cryptocurrency.
It is highly mined with cpu or gpu.
Pool Mining is the most common way to mine Monero.

Monero community is very active on IRC.
This document is the FAQ of the #monero-pools channel on Freenode IRC network.
You will find answer to the most common questions asked on this channel, related to monero mining, pool management, pool development.

## Questions and Answers

*### i have different machines mining, should i point them to same wallet? or will that confuse the pool?

The short answer is : use same address on all your miner. 
The wallet address is just used by pool to identify you and associate the number of share you submitted. 
Most of the pool have payement treeshold, so if you one address only, all your work will be associated to it, and you will reach the payement treeshold faster.
You can still use different address, pool doesn't mind, but it will slower your payement as far as the same amount of share will be spread around all your submitted wallet address. 

### I mine since few time, but my balance is still zero

In the current pool code, the balance is only updated when the pool discoverd a new block, and you submitted work for it. 
On small pool, it can take a few hours or even days to discover a new block. So your balance can stay the same for the same time. 

But keep in mind that whatever pool (big or small) you mine, once a block is discovered you will get almost same reward. 
For example instead of having 0.3xmr par day on big pool, you will receive around 3xmr every 10 days. 
But it can be stressfull to wait 10 days with a 0 balance indicator.

### when I will get my monero ?

You will get your monero once your balance reach the payment treeshold, and when the next payement batch will run. 
Depending of pool, payement batch is run every 6hours (it should be indicated on the pool website). 

### Can I get paid on market wallet directly ?

It depends of the pool. Some of them support this feature. 
Be very cautiaus to use the payement ID provided by the market, as far as it is the only way for the market that the transfered fund belongs to you

### How can I check if the balance is updated?

Refreshing the pool webpage should be enough

### why do so many monero pool sites have very similar layout is their an open source git or something?

Yes most of pools share the same code base : https://github.com/zone117x/node-cryptonote-pool
This was kindly coded by Zone11x. 
Also some fork with improvement exists, but rarely on the frontend which is what you mostly see and compare.

### hy can someone help me? My account is showing transfer founds but nothing is showing up in my wallet?

Try to refresh your wallet

### What graphics card are you using?

### Wolf0 are you the famous miner developper ?

Be careful to verify that the user you are talking with is a registered user. If so, there are 99.9% chance that he is the one you are thinking about. 
So scammer plays to impersonnate famous peoples, therefore always check before anything else. 

