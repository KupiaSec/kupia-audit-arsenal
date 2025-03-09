# What Is a VAMPIRE ATTACK? SUSHISWAP Saga Explained

*Upload Date: 20200912*

*Source: [https://www.youtube.com/watch?v=UFjXwrCGuog](https://www.youtube.com/watch?v=UFjXwrCGuog)*

# Understanding Vampire Attacks: The SushiSwap Saga

This article breaks down the concept of a "vampire attack" in the context of decentralized finance (DeFi), using the SushiSwap incident as a prime example. It explains the mechanics, incentives, and unforeseen consequences associated with this strategy.

## What is a Vampire Attack?

A vampire attack's primary goal is to attract liquidity away from an established DeFi platform (the "victim") to a new, competing platform.  This is achieved by incentivizing liquidity providers (LPs) from the target platform to stake their LP tokens on the new platform.

**The Steps:**

1.  **Incentivization:** The new platform(attacker) offers attractive rewards, typically in the form of its own native token, to LPs who stake their LP tokens (representing liquidity provided on the victim platform) on the attacking platform. This incentivizes liquidity providers to migrate.

2.  **Liquidity Migration:** Once sufficient liquidity has been attracted through staking, a smart contract (often called a "MasterChef" contract in these scenarios) is triggered. The MasterChef migrates the staked LP tokens from the victim platform to the new platform.

3.  **Utilization:** Since the staked LP tokens now represent the original liquidity in attacker's hand, allowing it to offer liquidity at it self. And it generates trading volume, and grow its user base.

## The SushiSwap Attack on UniSwap: A Case Study

SushiSwap launched on August 28th, 2020, amidst the DeFi summer craze. It aimed to compete directly with UniSwap by forking (copying) its code and implementing a vampire attack strategy.

**Key Aspects of the SushiSwap Attack:**

*   **Forked Code:** SushiSwap started by copying UniSwap's smart contract code, providing a functional duplicate of the platform.
*   **SUSHI Token Rewards:** Liquidity providers of UniSwap were incentivized to stake their UniSwap LP tokens on SushiSwap.  In return, they would receive SUSHI tokens of 1000 $SUSHI per Ethereum Block for a certain period.
*   **MasterChef Contract:** The heart of the attack was the MasterChef contract. This contract was designed to migrate the staked UniSwap LP tokens to SushiSwap after accumulating a certain amount of them.
*   **Admin Key and Timelock:** Initially, the SushiSwap founder("Chef Nomi") held the admin key to the MasterChef contract which caused a lack of trust. Chef Nomi solved it by creating a 48-hour timelock to trigger any admin functions.
*   **Liquidity Migration:** On September 9th, 2020, the migration was executed. Approximately $840 million worth of LP tokens were moved from UniSwap to SushiSwap.
*   **Aftermath:** Chef Nomi sold his $SUSHI which caused even more distrust. And then Chef Nomi returned the control to SBF(Sam Bankman-Fried) of FTX so that control of the project could safely reside there. Chef Nomi returned all of the $ETH he gained after getting caught, and apologized to the community.

## Technical Nuances

*   **Liquidity Pools:**  Sushiswap offered initial high APYs (Annual Percentage Yields), of between 200 to 1000 percent, for pools, such as: `SNX`, `EAT`, `LAND`, `EATH`, `WIFI`, `LINK`
*   **LP Tokens as Representation:** It's important to remember that LP tokens represent a provider's share of a liquidity pool. Staking these tokens on SushiSwap essentially gave SushiSwap control over that liquidity, even while it was technically still residing within UniSwap pools.
*   **Automated Market Makers (AMMs):** A vampire attack is effective because AMMs rely heavily on liquidity. By incentivizing liquidity migration, vampire attacks can cripple the original AMM.

## Unforeseen Events

The SushiSwap saga was far from a straightforward success story.

*   **Chef Nomi's actions:** The anonymous founder ("Chef Nomi") selling a huge portion of his $SUSHI holdings raised significant concerns.
*   **Control Transfer:**  The community essentially forced Chef Nomi to give up control of the project and hand administrative keys to FTX's Sam Bankman-Fried(SBF).
*   **Return of Control and Apologies:** Chef Nomi returned and refunded 14 million USD worth of $ETH.

## Conclusion

The SushiSwap vampire attack demonstrated the power of incentives and the ease with which liquidity could be moved between DeFi platforms. While initially successful in attracting liquidity away from UniSwap, the SushiSwap project faced a number of crises related to governance and trust. Despite a few up-and-down waves, SushiSwap remained one of the standard Automated Market Makers (AMM) in the space.