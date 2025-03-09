# How Does THORCHAIN Work? DEFI Explained

*Upload Date: 20210517*

*Source: [https://www.youtube.com/watch?v=dNDh-mPboPc](https://www.youtube.com/watch?v=dNDh-mPboPc)*

Okay, here's a blog article summarizing the YouTube video "How Does THORChain Work? DEFI Explained," based on the provided transcript, formatted in Markdown, and focusing on technical details:

# How THORChain Enables Native Cross-Chain Swaps: A Deep Dive

THORChain is a decentralized liquidity protocol that allows users to swap *native* assets across different blockchains *without* wrapping or pegging. This is a significant advancement over existing decentralized exchanges (DEXs) like Uniswap, Sushiswap, or Curve, which primarily operate within a single ecosystem (e.g., Ethereum) and require wrapped tokens for cross-chain interactions.  This article delves into the core mechanisms that make THORChain's cross-chain swaps possible.

## The Problem with Existing DEXs and Wrapped Tokens

Traditional DEXs, while powerful, are limited to assets within their native blockchain.  To trade Bitcoin on Uniswap, for instance, you'd need Wrapped Bitcoin (WBTC), an ERC-20 token representing Bitcoin on the Ethereum blockchain.  Wrapped tokens introduce trust assumptions and complexities:

*   **Custody:**  Someone (often a centralized entity) must hold the native Bitcoin and mint the corresponding WBTC.  This creates a single point of failure.
*   **Security:** The security of the wrapped asset is dependent on the security of the wrapping mechanism and the custodian.
*   **Complexity:** Users need to understand the wrapping/unwrapping process, adding friction.

THORChain aims to eliminate the need for wrapped assets altogether, allowing direct swaps between native L1 assets like BTC, ETH, BNB.

## THORChain's Core Components and Mechanisms

At its heart, THORChain is a network of nodes built using the Tendermint consensus engine and the Cosmos SDK.  This provides a robust and secure foundation.  Here's a breakdown of the key components:

1.  **THORChain Blockchain:**  This is a separate blockchain, *not* built on Ethereum. It has its own consensus and network layer, thanks to Tendermint and Cosmos SDK. This allows THORChain to operate independently and integrate with multiple blockchains.

2.  **THORNodes:** These are the validator nodes of the THORChain network. Each THORNode runs several critical services:
    *   **THORChain Service:**  This runs the THORChain blockchain itself (recording transactions, managing state, etc.).
    *   **Full Node of Connected Chains:**  Each THORNode runs a full node for *each* of the blockchains THORChain supports (e.g., a Bitcoin full node, an Ethereum full node, etc.).  This allows the nodes to *directly* observe transactions on those chains.
    *   **Bifröst Protocol:** This is the "connective layer" that links the THORChain network to the external blockchains.  It's responsible for watching vault addresses, observing inbound transactions, converting them into "witness" transactions on the THORChain, and constructing/broadcasting outbound transactions.

3.  **Vaults:** These are multi-signature addresses (or, more accurately, Threshold Signature Scheme addresses) on the *external* blockchains (e.g., a Bitcoin address controlled by the THORChain network).  There are two types:
    *   **Inbound Vaults:** These are the primary vaults that hold the majority of the funds.  They are more secure but slower, requiring a 2/3 majority of TSS signers to authorize a transaction (taking up to 20 seconds).
    *   **Outbound Vaults:**  These are smaller, less secure vaults run by *each* THORNode individually. Only a single signature from the node is required.  They hold a limited amount of funds (capped at 25% of the node's bond) to facilitate faster outbound transactions.  The funds in these vaults are constantly topped up from the inbound vaults.

4.  **Threshold Signature Scheme (TSS):**  This is a *crucial* security mechanism.  Instead of storing private keys on individual nodes (which would be a massive security risk), THORChain uses TSS.  TSS is a cryptographic primitive for distributed key generation and signing.  It's like an advanced multi-signature scheme, but crucially:
    *    It works at the *protocol* level, not the application level (like smart contract-based multisig).
    *   It offers better security and potentially lower transaction costs than traditional multisig. To sign a transaction, a threshold number of THORNodes (e.g., 2/3) must *collaboratively* generate a signature *without* ever reconstructing the full private key in one place.

5.  **Continuous Liquidity Pools (CLPs):** THORChain uses a liquidity pool model similar to Uniswap, but with a critical difference: *all* pools are paired with RUNE, THORChain's native token.  This means there's a BTC/RUNE pool, an ETH/RUNE pool, etc.  This simplifies routing.  A swap from BTC to ETH goes through two pools: BTC/RUNE, then RUNE/ETH.

6.  **RUNE Token:** The RUNE token serves multiple critical roles:
    *   **Liquidity Pairing:**  As mentioned, RUNE is paired with every asset in the liquidity pools.
    *   **Security (Bonding):** THORNodes must "bond" (stake) a significant amount of RUNE to participate in the network. This bond is at risk if the node misbehaves (e.g., attempts to steal funds). The bond required is *1.5 times* the value of the assets the node helps secure in the outbound vaults.
    *   **Incentive Pendulum:** This mechanism aims to keep the system in an optimal state where 67% of RUNE is bonded and 33% is in liquidity pools.
    *   **Governance:** RUNE holders can participate in governance, signaling which chains and assets should be added to the network.
    *    **Transaction Fees**: Pay for gas needed for outbound transactions.

7.   **Churning:** It is the process to maintain a healthy, secure node set for THORChain's network.
    * Every 5,000 blocks is about three days:
        *   The churning process starts.
        *   The oldest and lower-performing nodes are replaced with nodes on standby.
     It ensures new nodes can enter the network for transaction validation, and it rotates node ownership of vaults for enhanced security, as active nodes move funds to new vaults controlled by the incoming nodes.

## The Swap Process: A Step-by-Step Example (BTC to ETH)

1.  **User Sends BTC:** The user sends a standard Bitcoin transaction to a Bitcoin vault address controlled by the THORChain network.

2.  **Nodes Observe:** THORNodes, running full Bitcoin nodes, monitor the vault addresses and detect the incoming transaction.

3.  **Bifröst Conversion:** The Bifröst protocol on the THORNodes converts the observed Bitcoin transaction into a "witness" transaction on the THORChain blockchain.

4.  **Consensus and Finalization:** The THORNodes reach consensus on the witness transaction.  Once the majority agrees, the transaction is moved to a "finalized" state. This records the user's Bitcoin deposit on the THORChain.

5.  **Swap Initiation:** The THORChain protocol initiates the swap (BTC for RUNE, then RUNE for ETH) using the Continuous Liquidity Pools.

6.  **Outbound Transaction:** The Bifröst protocol is used *again*, this time to initiate a withdrawal of ETH from the Ethereum outbound vault.

7.  **Translation and Broadcast:** The outbound transaction is translated from THORChain's internal representation into a valid Ethereum transaction and broadcast to the Ethereum network.

8.  **Completion:** The user receives ETH in their Ethereum wallet.

## Impermanent Loss Protection

THORChain offers 100% impermanent loss protection (ILP) for liquidity providers that remain staked for at least 100 days.
Protection starts at 1% per day, so a provider staked for 30 days has 30% ILP protection.

## Key Advantages of THORChain

*   **Native Asset Swaps:** No need for wrapped tokens, reducing complexity and trust assumptions.
*   **Decentralized:**  The network is controlled by a distributed set of nodes, with strong economic incentives for honest behavior.
*   **Cross-Chain:** Supports multiple blockchains, enabling a truly interconnected DeFi ecosystem.
*   **Security:** Leverages TSS for secure vault management 
*   **Incentive Alignment:** The RUNE token and the incentive pendulum align the interests of node operators, liquidity providers, and traders.

## Potential Limitations and Considerations

*   **Complexity:**  The underlying technology is complex, which can make it challenging to understand and audit.
*   **TSS Reliance:** While TSS is promising, it's a relatively newer technology compared to more established cryptographic primitives.
*   **Economic Security:** The security of the system relies heavily on the economic incentives provided by the RUNE token and the bonding mechanism.  A significant drop in RUNE's price could potentially weaken security.
*   **Not Fully Composable (Yet):** Unlike Ethereum-based DEXs, THORChain swaps are not easily composable within single transactions. This is because THORChain is its own blockchain.
*   **Decentralization Level:** While more decentralized than centralized exchanges, THORChain is still less decentralized than Bitcoin or Ethereum themselves.

## Conclusion

THORChain presents a novel and ambitious approach to solving the cross-chain liquidity problem in DeFi. By enabling native asset swaps without wrapping, it offers significant advantages in terms of user experience, security, and trust minimization. However, it's a complex system, and its long-term success will depend on the continued robustness of its technology, the strength of its economic incentives, and the growth of its ecosystem.