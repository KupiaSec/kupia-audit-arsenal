# How do LIQUIDITY POOLS work? (Uniswap, Curve, Balancer)

*Upload Date: 20200720*

*Source: [https://www.youtube.com/watch?v=cizLhxSKrAc](https://www.youtube.com/watch?v=cizLhxSKrAc)*

# Understanding Liquidity Pools: Uniswap, Curve, and Balancer

Decentralized Finance (DeFi) has revolutionized traditional financial systems by enabling peer-to-peer trading and lending without intermediaries. A core component of many DeFi platforms is the Liquidity Pool (LP). This article explore how liquidity pools work, focusing on popular platforms like Uniswap, Curve, and Balancer.

## What are Liquidity Pools?

Liquidity pools are essentially smart contracts holding a reserve of two or more tokens, creating liquidity for trading. They are used by decentralized exchanges (DEXs) to facilitate trading without relying on traditional order books. Instead of matching buy and sell orders, traders execute trades directly against the pool's reserves. Liquidity providers (LPs) deposit their tokens into the pool and earn fees generated from the trading activity.

## How Liquidity Pools Work

Here's a breakdown of the typical process:

1.  **Liquidity Provision:**
    *   Liquidity providers (LPs) contribute equal values of two tokens to the pool (e.g., ETH and DAI). This initial deposit determines the pool's initial ratio and starting price.
    *   In return, LPs receive LP tokens, representing their share of the pool.
2.  **Trading:**
    *   Traders swap tokens against the pool's reserves.
    *   Since there are equal values only, if token A in the liquidity pool can be traded for token B using formula `x * y = k` where `x` is the amount of token A, `y` amount of token B and `k` remain constant.
    *   Each trade incurs a small fee that is distributed proportionally to LPs based on their LP token holdings.
3.  **Price Determination:**
    *   The price of tokens in the pool is determined by the ratio of the tokens in the pool and price changes depending on the size of the trade.
    *   Large trades can cause significant price slippage, while smaller trades have minimal impact.
4.  **Earning Fees:**
    *   Fees generated from each trade are accumulated in the pool.
    *   LPs can redeem their LP tokens to claim their proportional share of the accumulated fees, alongside their original deposit.

## Key Concepts

*   **Impermanent Loss (IL):** A major risk for LPs. IL occurs when the price ratio of the tokens in the pool changes after the LP has deposited their tokens. The LP might have been better off simply holding the tokens outside the pool. The more significant the price divergence, the greater the IL.
*   **Slippage:** The difference between the expected price and the actual price at which a trade executes. Higher slippage occurs when the trade size is large, relative to the pool's liquidity.
*   **Automated Market Maker (AMM):** The underlying protocol that defines how prices are determined and trades are executed within a liquidity pool. Uniswap, Curve, and Balancer are all AMMs, each with different mechanisms and targeted assets.

## Platform Specifics
Each AMM has distinct characteristics.
### Uniswap
Uniswap pioneered the `x * y = k` AMM model. This implies that the total supply at all time must result a constant `k`.
*   **Focus:** General-purpose AMM suitable for a wide variety of tokens.
*   **Pricing Function:**  `x * y = k` (Constant Product). This formula balances token liquidity according to total supply.
*   **Use case:** Best suited for trading pairs where volatility is expected.
### Curve
Curve specializes in efficient stablecoin swaps and assets that have low price volatility like wrapped bitcoin tokens. The key difference is in its formula which aim to maintain a constant sum instead of product.
*   **Focus:** Stablecoin swaps.
*   **Pricing Function:** Hybrid of constant product and constant sum, optimized for stablecoin pairs.
*   **Use case:** For example, swapping USDC for USDT, Curve provides the highest efficiency with minimal slippage.
### Balancer
Balancer allows the liquidity pool to have many different tokens to create custom portfolios that self-balance.
*   **Focus:** Custom pools with multiple tokens (more than 2).
*   **Pricing Function:** Generalization of `x * y = k` with weighted token ratios.
*   **Use case:** Balancer allows the creation of index-fund-like pools, where weightings automatically adjust based on trading activity.

## Risks of Liquidity Pools

*   **Impermanent Loss:** As described above, a major concern for LPs.
*   **Smart Contract Risk:** Vulnerabilities in the smart contract code can lead to loss of funds.
*   **Rug Pulls:** In pools with less reputable tokens, developers can drain the pool, leaving LPs with worthless tokens.
*   **Volatility** High volatility can increase risks.

## Conclusion

Liquidity pools are essential to DeFi as an incentive to increase trading volume on decentralized exchanges. Platforms like Uniswap, Curve and Balancer provide distinct advantages depending on the assets held or traded. Understanding LP risks like impermanent loss and selecting secure/audited platforms are vital before getting involved.