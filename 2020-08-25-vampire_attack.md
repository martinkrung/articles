# Vampire Attack (Vampire Mining) - an attack on liquidity dependent protocols

Here we have dark scenario for liquidity dependent projects called the vampire attack. In the interest of keeping DeFi projects secure and behaving as intended, liquidity lock-up or sufficient time-based rewards for locking up liquidity provider should be implemented. This attack uses [migration mining](https://www.cryptonative.ch/migration-mining-mm-a-new-form-of-incentive-for-crypto-projects-to-get-liquidity-into-a-liquidity-dependent-protocol/ "migration mining").

## Simple Vampire Attack

1. Clone a project A (from its smart contracts to even its front-end). Project A has no token yet, but earns fees on token volume.
2. Implement migration mining from project A to project B. Simply, give $b to people who migrate liquidity from A to B.
3. Implement governance and start sharing revenue to tokenholders holding $b.
4. Attack will be successful if Project A is drained of sufficient liquidity.

## Advanced Vampire Attack

A combination of migration mining, leverage shorting Project A's tokens ($a) and going leverage long Project B's tokens ($b).

1. Capital accumulation: sell $vampire over a bonding curve end get $usd into treasury.
2. With 1/2 of the treasury you go to a lending market and lend as much $a as you can.
3. With the other part you buy $b and put it into lending to leverage long (buying more $b)
4. Implement migration mining from project A to project B. Simply, give $vampire to those who migrate liquidity from A to B. In parallel start selling $a to lower the price. With a portion, leverage up by lending more $a on a lending market and sell this too. With the other portion, buy more $b from project B.
5. People start migrating liquidity from project A to B to earn $vampire. The price of $a is expected to crash (because without liquidity, the project is worthless and has no revenue). Expect the price of $b to start rising.
6. Now buy back the now worthless $a, pay off the incurred debt, and get your initial $usd with leverage back and put it into the treasury.
7. Distribute the $usd and $b to the people having $vampire

## A Vampire Attack is a simple "hack" but has wide implications:

- The era of free liquidity flow is over. Liquidity migration itself has to be rewarded as  [migration mining](https://www.cryptonative.ch/migration-mining-mm-a-new-form-of-incentive-for-crypto-projects-to-get-liquidity-into-a-liquidity-dependent-protocol/ "migration mining").

- Projects will have to pay for liquidity lock-up rather than contend with free floating liquidity
- Liquidity owners can become protocol owners with no or little risk
- Shorting/Longing entire projects are now possible with this strategy (Advanced Vampire Attack)
- Advanced Vampire Attacks share characteristics with flash loan attacks but is slower
- Private owned projects who are liquidity dependent have a high risk of vampire attacks
- Every liquidity dependent project needs lock-up periods or a form of compounding rewards for long-term liquidity provider



## Executive Summary for non crypto people

Imagine two traditional banks (A and B) which have similar services. 

B is very new and has no liquidity. So B decides to distribute shares and a reward for the liquidity you bring in. B knows that A is dependent on liquidity, as is every bank. So B takes out a loan somewhere, buys shares of A (with leverage) and sells these on the market. 

Then B tells every customer of A that it has a plan to suck out A's liquidity, distribute its own shares, and offer a reward as incentivization. If successful, people will start to migrate liquidity from A to B. (Incoming liquidity would have a lock-up period and you would receive more shares the longer you lock-up)  

A cannot stop liquidity outflow because customers can do this electronically without permission. This results in A going bust and the value of A's shares drops to zero. To finalize the scheme, B pays back the now worthless shares from A and distributes the profits as rewards for its own shareholders.



Tweet from 2020-08-25 about the vampire attack: https://twitter.com/martinkrung/status/1298363320270032897?s=20
Many thanks to [Daniel Hwang](https://twitter.com/danhwang88 "Daniel Hwang") for corrections.

