# monero-pool-faq
<!-- vim-markdown-toc GFM -->
* [General purpose of this document](#general-purpose-of-this-document)
* [Questions and Answers](#questions-and-answers)
    * [I Have Different Machines Mining, Should I Point Them To Same Wallet? Or Will That Confuse The Pool?](#i-have-different-machines-mining-should-i-point-them-to-same-wallet-or-will-that-confuse-the-pool)
    * [I mine since few time, but my balance is still zero](#i-have-been-mining-for-some-time-now-but-my-balance-is-still-zero)
    * [When I will get my Monero ?](#when-i-will-get-my-Monero)
    * [Can I get paid on market wallet directly ?](#can-i-get-paid-on-market-wallet-directly)
    * [How can I check if the balance is updated?](#how-can-i-check-if-the-balance-is-updated)
    * [Why do so many Monero pool sites have very similar layout is their an open source git or something?](#why-do-so-many-Monero-pool-sites-have-very-similar-layout-is-their-an-open-source-git-or-something)
    * [Who can someone help me? My account is showing transfer founds but nothing is showing up in my wallet?](#who-can-someone-help-me-my-account-is-showing-transfer-found-but-nothing-is-showing-up-in-my-wallet)
    * [What graphics card are you using?](#what-graphics-card-are-you-using)
    * [Wolf0 are you the famous miner developer ?](#wolf0-are-you-the-famous-miner-developer)

<!-- vim-markdown-toc -->


## General purpose of this document

Monero is a new generation cryptocurrency.
It is highly mined with cpu or gpu.
Pool Mining is the most common way to mine Monero.

Monero community is very active on IRC.
This document is the FAQ of the #Monero-pools channel on Freenode IRC network.
You will find answer to the most common questions asked on this channel, related to Monero mining, pool management, and pool development.

## Questions and Answers

### I have different machines mining, should I point them to same wallet? or will that confuse the pool?

The short answer is: Use the same address on all your miners. 
The wallet address is used by pool to identify you and associate the number of shares that you have submitted.
Most of the pools have payment thresholds, so if you use only one address, all your work will be associated with it, and you will reach the payment threshold faster.
You can still use different address, the pools don't mind, but it will slow down your payments as the same amount of shares will be spread around all your submitted wallet addresses.

### I have been mining for some time now, but my balance is still zero!

In the current pool code, the balance is only updated after the pool discovers a new block, assuming that you submitted work for that block.
On small pool, it can take a few hours or even days to discover a new block, as such your balance can stay the same for a longer period of time.
But keep in mind that whatever pool (big or small) you mine, once a block is discovered you will get almost same reward. 
For example instead of having 0.3xmr par day on big pool, you will receive around 3 XMR every 10 days.
But it can be stressful to wait 10 days with a 0 balance indicator.
Blocks also only unlock after the block is a particular age, and balances are not increased until this is hit.

### When I will get my Monero?

You will get your Monero once your balance reaches the payment threshold, then once the pool runs the next payment batch.
Depending of pool, payment batch is run every 6hours (it should be indicated on the pool website). 

### Can I get paid on market wallet directly?

It depends of the pool. Some of them support this feature. 
Be very careful to use the exact payment ID provided by the market, as it is the only way for the market that the transferred funds belongs to you!

### How can I check if the balance is updated?

Refreshing the pool webpage should be enough

### Why do so many Monero pool sites have very similar layout is their an open source git or something?

Yes most of pools share the same code base : https://github.com/zone117x/node-cryptonote-pool
This was kindly coded by Zone11x. 
Also some fork with improvement exists, but rarely on the frontend which is what you mostly see and compare.

### Who can someone help me? My account is showing transfer found but nothing is showing up in my wallet?

Try to refresh your wallet

### What graphics card are you using?

### Wolf0 are you the famous miner developer?

Be careful to verify that the user you are talking with is a registered user. If so, then there is a 99.9% chance that he is the one you are thinking about.
Scammers often work to impersonate famous people within channels, therefore always check before anything else.

