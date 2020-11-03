# Vampire Attack (Vampire Mining) - an attack on liquidity dependent protocols

I did just come up with a very dark scenario for liquidity dependent projects. It's call the vampire attack! No, garlic will not save your project! To protect your defi project, you should as soon as possible implement some form of liquidity lock-up or reward long term liquidity provider. This attack uses [migration mining](https://www.cryptonative.ch/migration-mining-mm-a-new-form-of-incentive-for-crypto-projects-to-get-liquidity-into-a-liquidity-dependent-protocol/ "migration mining").

## Simple Vampire Attack to bootstrap your project B

1. Copy project A with all its open sourced smart contract and front-end. A has no token yet, but earns fee on every token flow.
2. You implement migration mining from project A to project B, basically you give $b to people who migrate liquidity from A to B.
3. You implement some governance and start sharing revenues to your new tokenholders holding $b.
4. Project A has no liquidity and loses all revenue

## Advanced Vampire Attack

It's a combination of migration mining, leverage shorting $a and going leverage long $b.

1. Capital accumulation: You sell $vampire over a bonding curve end get $usd in your treasury.
2. With 1/2 of the treasury you go to a lending market and lend as much $a as you can.
3. With the other part you buy $b and put it into lending to leverage long (buying more $b)
4. You implement migration mining from project A to project B, basically you give $vampire to poeple who migrate liquidity from A to B. In parallel you start selling $a to the market to lower the price. With part of the money you leverage up, lending more $a on a lending market and selling this too. With the other part you buy more token from project B.
5. People start to migrate liquidity from project A to B to earn $vampire, price of $a is crashing, because without liquidity project is worthless and has no revenue. Price of $b starts raising.
6. You buy back the now worthless $a and pay off your dept, get your initial $usd with leverage back and put it into the treasury.
7. You distribute the $usd and $b to the people having $vampire

## A Vampire Attack is a quite simple "hack" but has wide implications:

- Time of free liquidity flow is over. Liquidity migration itself has to be rewarded as  [migration mining](https://www.cryptonative.ch/migration-mining-mm-a-new-form-of-incentive-for-crypto-projects-to-get-liquidity-into-a-liquidity-dependent-protocol/ "migration mining").

- Project will have to pay liquidity who is lock-up different then free floating liquidity
- Liquidity owner can become protocol owner without or little risk
- Shorting/Longing whole project is possible with this, also from outsider (Advanced Vampire Attack)
- Advanced Vampire Attack has some characteristic with a flash loan, but its way slower
- Private owned project who are liquidity dependent have a high risk for vampir attack
- Every liquidity dependent project needs some lock-up period or some form of compounding reward for long term liquidity provider



## Executive Summary for non crypto people

Imagine two traditional banks A and B which have very similar service. B is very new and has no liquidity. So B decides to distribute shares and a reward for the liquidity you bring in. B knows that A is dependent on liquidity, as every Bank. So B takes out a loan somewhere, buys shares of A (with levarage) and sell these on the markets. Then B tells every costumer of A, that they have got this plan to suck liquidity out of A, distribute its own shares and some reward on top. So people start to migrate liquidity from A to B. (Incomming liquidity has a lock-up period and you get more shares the longer you lock-up)  A cannot stop liquidity outflow, because costumers can do this electronically without permission. Result A goes bust and value of shares drops to zero. Then B pays back the now worthless shares from A and distributes the gain as reward for there own shareholders.
