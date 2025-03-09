# What Is BANCOR V2? CHAINLINK Integration And Dynamic Automated Market Maker Explained

*Upload Date: 20200810*

*Source: [https://www.youtube.com/watch?v=bWBfLArJsFk](https://www.youtube.com/watch?v=bWBfLArJsFk)*

# Bancor V2: A Deep Dive into Chainlink Integration and the Dynamic Automated Market Maker

Bancor V2 aims to compete with other decentralized exchanges like Uniswap, Curve, and Balancer, and uniquely integrates with Chainlink. This blog post details the key aspects of Bancor V2, with focus on its Dynamic Automated Market Maker (DAMM) and its use of Chainlink oracles.

## What is Bancor?

Bancor is an on-chain liquidity protocol designed to enable automated, decentralized token exchange on Ethereum and across blockchains. Launched in 2017 with one of the largest ICOs, the protocol is built upon smart contracts allowing for peer-to-contract trades in a single transaction, eliminating the need for a counterparty..  Users deposit liquidity into automated market makers (AMMs) in exchange for trading fees, staking rewards, and voting rights within the Bancor DAO.

## Addressing the Challenges of AMMs

Bancor V2 addresses several key obstacles hindering the wider adoption of AMMs:

*   **Impermanent Loss:** The most significant challenge, impermanent loss, arises from the fixed ratio between tokens in standard liquidity pools as external prices fluctuate. Arbitragers rebalance the pool, extracting profit that would otherwise accrue to the liquidity provider (LP).
*   **Exposure to Multiple Assets:** Traditional AMMs require LPs to provide both assets in a pool.
*   **Capital Inefficiency:** Capital inefficiencies arise due to fixed weighting. This is adressed with bonding curve in V2.
*   **Opportunity Cost of Providing Liquidity:** Opportunity cost occurs as capital is tied for longer time in system.

## Bancor V2: Key Features

Bancor V2 introduces several key features to overcome these obstacles, most notably a **Dynamic Automated Market Maker (DAMM)**.

### Dynamic Automated Market Maker (DAMM)

DAMMs aim to address impermanent loss and multi-asset exposure. In essence, *impermanent* loss is the *temporary* loss while funds are in the AMM, arising from holding asset vs HODLing asset. Impermenant loss arises due the fixed ratio of the two tokens in liquidity pool, it forces rely on arbitragers.

DAMMs leverage price oracles (like Chainlink) to dynamically balance the ratio of tokens in a pool.

#### How DAMMs Work

1.  **Initial Balanced State:** v2 pools are initialised by arbitragers, ensuring accurate pricing at start.
2.  **Price Updates from Oracles:** DAMMs rely on price oracles with the Chainlink to tell balances in the pool.
3.  **Dynamic Weight Adjustments:** When the price changes, weights of each token adjust. With price increases, target weight would grow.
4.  **Mitigating Impermanent Loss through Dynamic Fees:** By using dynamic fees, DAMMs create incentives for traders to rebalance weights, ensuring LPs can withdraw the number of tokens they initially provided, thus mitigating impermanent loss.
5.  **Single Asset Provision:** DAMMs permits LPs to add liqidity for each individual pool, which decreases risks.

### Integration with Chainlink Oracles

Dynamic fee ajustments is used within the market participant. When prices increase target wights changes. Oracle does all of this through Chainlink. With Chainlink, protocol can bring more efficient bonding curve. This occurs by giving LPs decentralized and reliable prices to smart contracts to make trading as fair as possible.

### Capital Efficiency

Bonding curves are used to decrease capital inefficiencies. This helps with decrease slippage. DAMMs provide more capital efficient staking and liquidity providing then V1 systems.

## Tradeoffs

*   **Bnt Still Needed:** V2 pool still rely on BNT still, making it less versataile then uniswap.
*  **Two Token Limits:** V2 pool has two tokens, which limit balancer.

# Conclusion

Bancor V2 is a significant upgrade, aiming to provide solutions to some of the core challenges facing AMMs. By integrating Chainlink and introducing DAMMs, Bancor seeks to give LPs greater flexibility, decrease impermanent loss, and improves capital efficiency. The unique features of Bancor V2 makes it promising but it also needs improve to complete with some main competitors like curve and uniswap.