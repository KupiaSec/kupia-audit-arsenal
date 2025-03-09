# Ethereum LAYER 2 SCALING Explained (Rollups, Plasma, Channels, Sidechains)

*Upload Date: 20201027*

*Source: [https://www.youtube.com/watch?v=BgCgauWVTs0](https://www.youtube.com/watch?v=BgCgauWVTs0)*

# Ethereum Layer-2 Scaling Explained: Rollups, Plasma, Channels And Sidechains

Ethereum scaling has been a hot topic since its launch, particularly during periods of network congestion, such as the 2017 Crypto Kitties craze and the DeFi boom of 2020; these events lead to high gas fees, sometimes exceeding $500 which made transactions prohibitively expensive.

## Scaling Ethereum: Layer-1 vs. Layer-2

There are two main approaches to scaling a blockchain, including Ethereum:

*   **Layer-1 Scaling (On-Chain):** Improving the base layer itself, like upgrading the Ethereum protocol directly which involves changes such as Proof-of-Stake and Sharding.
*   **Layer-2 Scaling (Off-Chain):** Building additional layers on top of the base layer to handle transactions and computations, offloading the work from Layer-1.

Layer-2 solutions are built on top of Layer-1, leveraging the security of Layer-1 by anchoring the state into Layer-1. Ethereum can process ~15 transactions per seconds on Layer-1 right now, while Layer-2 scaling can dramatically increase this number. Depending on the solution, processing between 2000 and 4000 transactions per second is possible. While Ethereum 2.0 introduces Proof-of-Stake and Sharding which dramatically increases transaction throughput on the base layer, Layer-2 scaling is still required. The famous scalability trilemma comes into play. Skipping Layer-2 and only focusing on Layer-1 would require specialized nodes to handle the increased workload, leading to higher centralization and losing security and censorship resistant properties of the network.

Layer-2 scaling encompasses solutions increasing Layer-1's capabilities by handling transactions off-chain for improved transaction speed and throughput.

Ultimately, Layer-2 aims to reduce gas fees for actual scaling solutions. Some options are available, whilst others are aiming for a medium to long-term time horizon.

## Popular Ethereum Layer-2 Scaling Solutions

Here's breakdown of some of the popular Ethereum Layer-2 scaling solutions:

*   **Channels:** Enable participants to exchange transactions multiple times while only submitting two transactions to the base layer. They are application-specific and require participants to be known upfront, also requiring users to lock up funds in a multi-sig contract on top of it, which is restrictive in nature. Their main benefit is fast transactions. Raiden Network (Ethereum) and Lightning Network (Bitcoin) are examples.
    *   **State Channels:** This is the broad category of channels, encompassing various subtypes, including payment channels.
    *   **Payment Channels:** Focused specifically on payment transfers between participants.
*   **Plasma:** A framework for building scalable applications on Ethereum, using smart contracts and Merkle trees to create an unlimited number of "child chains" (copies of the parent Ethereum blockchain), offloading transactions from the main chain. Drawbacks include a long waiting period for users withdrawing funds, and not supporting general-purpose smart contracts which limits it to simple payments. OMG Network (Matic Network) is an implementation of Plasma.
*   **Sidechains:** Ethereum-compatible, independent blockchains with their consensus models and block parameters. Interoperability with Ethereum made possible by the Ethereum Virtual Machine (EVM), allowing contracts deployed to Ethereum to be directly deployed to the sidechain. xDAI is an example.
*   **Rollups:** Provide scaling by bundling a number of sidechain transactions. Sidechain transactions are rolled up into the a single transaction with cryptographic proof (SNARKs which is Succinct Non-Interactive Argument of Knowledge), submitting only that proof to base layer to save gas fees.
    *   **ZK-Rollups:** Use zero-knowledge proofs (SNARKs) for faster and more efficient processing.
    *   **Optimistic Rollups:** Transactions are assumed to be valid unless challenged where fraud proofs are then executed.
        *There are two types of Rollups: ZK-Rollups, and Optimistic Rollups.* ZK Rollups are faster and more efficient than Optimistic Rollups.

ZK Rollups, although faster and more efficient than Optimistic Rollups, existing smart contracts cannot easily migrate to Layer-2. Optimistic Rollups run an EVM-compatible virtual machine called OVM (Optimistic Virtual Machine) which allows for executing the same contracts as can be executed on Ethereum. This offers composability. Optimism does this; for ZK-roll-ups, there is Loopring, Diversify, and ZK-Sync.

Rollups can also be magnified by Ethereum 2.0, only needing the data layer to be scaled; and therefore, they can get a tremendous increase in performance.

Rollups and Ethereum 2.0 seems like an integrated Layer-2 solution for the future, with Ethereum converging. This was confirmed in Vitalik Buterin's recent post called "A roll-up centric ethereum roadmap".