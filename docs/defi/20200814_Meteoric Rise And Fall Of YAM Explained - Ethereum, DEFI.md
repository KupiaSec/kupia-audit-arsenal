# Meteoric Rise And Fall Of YAM Explained - Ethereum, DEFI

*Upload Date: 20200814*

*Source: [https://www.youtube.com/watch?v=DXUhD8m_KMc](https://www.youtube.com/watch?v=DXUhD8m_KMc)*

# Meteoric Rise and Fall of YAM Explained: An Ethereum DeFi Case Study

This blog post explores the YAM cryptocurrency project, a DeFi experiment on the Ethereum blockchain that experienced rapid growth followed by a critical failure, highlighting key lessons in smart contract development and decentralized governance.

## The Promise of YAM: A Rebase Token with Governance

YAM aimed to be a self-governing, yield-optimizing stablecoin. It was an experimental protocol designed to be community-led with no pre-mine, no pre-sale, and no venture capital allocation. The core features of YAM included:

*   **Rebasing:** YAM employed an elastic supply mechanism. It expanded or contracted supply based on market conditions to target a price of \$1. When the price of YAM was above \$1, the protocol increased the supply, distributing new tokens to holders (positive rebase). Conversely, When the price was below \$1, the protocol would shrink the supply (negative rebase). The goal is to bring price back to target.
*   **Yield Farming:** Users could earn YAM by staking other DeFi tokens like COMP, LEND, LINK, MKR, SNX, and WETH.
*   **Treasury and Governance:** A portion of each rebase was allocated to a treasury controlled by YAM holders through on-chain governance. Funds accumulated in treasury would be used towards various incentive or development plans.

## The Meteoric Rise (and TVL)

YAM's launch was met with overwhelming enthusiasm. Within 24 hours, over \$600 million worth of crypto assets were locked into the YAM protocol, demonstrating significant demand for decentralized stablecoins and yield farming opportunities.

## The Fatal Flaw: A Rebase Bug

The rapid success quickly unraveled. During the first rebase, a critical bug in the smart contract was discovered.  The bug was in the smart contract responsible for accumulating YAM to be used for governance (treasury). The contract intended to calculate and transfer a percentage of the rebase supply to the treasury. However, an error in the calculation resulted in the contract minting and sending **far more YAM to the treasury than intended**. The exact scenario being:

1. Each rebase, the contract calculated how much YAM needed to be transferred using this `amountToBeTransfered = rebaseAmount * votingRewardRate`,
2. `votingRewardRate` was supposed to be a factor between `0` and `1`. (e.g. `0.1` means 10%), and to prevent decimal operations, this was handled using integers as `10% = 10 / 100 => 100 = 1000`
3. The code accidentally multipled `votingRewardRate` one too many times such that the amount was extremely larger than expected.
4. This resulted in the allocation to governance being far more than initially proposed.

*   As a result, the rebase minted an enormous amount of new YAM and sent it to the treasury. Because the treasury contract didn't have safety measures built in, this action was allowed.

This event threatened the stability of the entire YAM ecosystem. The excess supply of YAM in the treasury effectively made it impossible for the governance process to function as designed.

## The Attempted Rescue: A Failed On-Chain Governance Vote

The YAM community quickly mobilized to find a solution. The development team proposed a plan to rescue the project:

1.  **Mint YAM:** Mint new YAM tokens and use them to purchase yCRV (Yearn Curve) tokens.
2.  **Governance Transfer:** Trigger a governance function in the yCRV contract to transfer ownership to the YAM community.
3.  **Burn Treasury YAM:** Burn the excess YAM sitting in the treasury contract in order to fix supply.

This process was put to a vote, however, due to slow blockchain congestion and the way the vote was structured, not enough community members participated to ratify the fix.

## The Fall: A Lesson in Decentralized Governance and Smart Contract Audits

With no viable solution to countermeasure the mistake with treasury fund allocations, the YAM project quickly collapsed. Its market price plummeted towards zero as users lost faith in the project's ability to recover.

The YAM incident served as a stark reminder of the risks associated with nascent DeFi projects and unaudited smart contracts. Key takeaways include:

*   **Smart Contract Audits are Essential:** Even seemingly minor coding errors can have catastrophic consequences. Thorough audits by experienced security firms are critical before deploying smart contracts with significant amounts of user funds. To avoid problems like YAM it helps to:
    *   Write tests for contract, consider edge cases
    *   Keep a mindset of healthy paranoia as opposed to simply "trust" the code works
    *   Consider a secondary audit after deploying code
*   **Decentralized Governance Challenges:** On-chain governance can be slow and inefficient. Participation rates can be low, and delays in decision-making can exacerbate problems.
*   **The Importance of Economic Modeling:** DeFi protocols require careful economic modeling and simulations to understand how they will behave under different market conditions. YAM's rebase mechanism, while theoretically sound, proved vulnerable to exploitation due to its lack of robust safeguards.
*   **Community Trust is Paramount:** The rapid collapse of YAM demonstrated how quickly trust can erode in DeFi. Transparency, clear communication, and a commitment to security are crucial for building and maintaining community confidence.

## YAM's Legacy: Learning from Failure

Despite its short lifespan, YAM left a lasting impact on the DeFi space. It highlighted the experimental nature of the industry, emphasized the importance of security and governance, and served as a valuable case study for future DeFi projects. Even though YAM failed, its legacy provides insights and direction for other projects in the future.