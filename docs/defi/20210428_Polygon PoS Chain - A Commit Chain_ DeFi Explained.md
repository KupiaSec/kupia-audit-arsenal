# Polygon PoS Chain - A Commit Chain? DeFi Explained

*Upload Date: 20210428*

*Source: [https://www.youtube.com/watch?v=f7F67ZP9fsE](https://www.youtube.com/watch?v=f7F67ZP9fsE)*

# Understanding Polygon PoS Chain: A Commit Chain?

## Introduction

The video titled "Polygon PoS Chain - A Commit Chain? DeFi Explained" delves into the intricacies of the Polygon PoS (Proof of Stake) Chain, particularly focusing on its unique features and how it differentiates itself from traditional sidechains. The discussion revolves around the concept of a "commit chain" and its implications for decentralized finance (DeFi).

## Sidechains vs. Commit Chains

### Sidechains

Sidechains are independent blockchain networks that operate alongside the main blockchain (like Ethereum) to enhance scalability. They have their own consensus mechanisms, often limiting the number of entities that can validate the chain. This can lead to a situation where only a select few are responsible for maintaining the network, which might compromise decentralization.

### Polygon PoS Chain

Polygon PoS Chain, however, introduces a novel approach by being a "commit chain." This term signifies that the chain is deeply integrated with the Ethereum mainnet, inheriting its security features. Unlike traditional sidechains, Polygon PoS Chain validators are not limited by a small, fixed set of authorities. Instead, anyone can join the network by staking Matic tokens, ensuring a more decentralized and secure system.

## Key Components of Polygon PoS Chain

### Heimdall and Bor

The architecture of Polygon PoS Chain is divided into two main components: Heimdall and Bor.

- **Heimdall**: This layer is responsible for checkpointing, which provides finality on the Ethereum chain. It aggregates blocks produced by Bor and periodically publishes them to the Ethereum mainnet. This process is known as checkpointing and is crucial for ensuring the security and integrity of the network.

- **Bor**: This layer allows for the aggregation of blocks and their subsequent publication to the Ethereum mainnet. It ensures that the network remains in sync with the Ethereum contract state at all times.

## Validator Selection and Security

### Validator Selection Process

Validators in the Polygon PoS Chain are selected using a weighted round-robin algorithm. This ensures a fair and decentralized selection process. The selection is based on the amount of Matic tokens staked by the validators. The more tokens staked, the higher the chances of being selected as a validator.

### Security Features

The Polygon PoS Chain contract deployed on the Ethereum mainnet is considered the ultimate source of truth. All validation is done by acquiring the Ethereum mainnet contract state. This ensures that the network is secured by the robust Ethereum blockchain.

## Two-Way Ethereum Bridge

The two-way Ethereum bridge in Polygon PoS Chain provides increased security guarantees. Unlike traditional bridges that rely on a small set of authorities, the Polygon PoS Chain bridge is secured by a robust set of validators whose state is maintained on the Ethereum mainnet. This makes it one of the few bridges secured by the entire validator set of a breached chain.

## Conclusion

Polygon PoS Chain offers a unique blend of scalability and security by leveraging the Ethereum mainnet. Its commit chain architecture, with components like Heimdall and Bor, ensures that it remains decentralized and secure. The video invites viewers to share their thoughts on the value of distinguishing Polygon PoS Chain as a commit chain and encourages engagement through likes, subscriptions, and support via Patreon.

This comprehensive overview of the Polygon PoS Chain highlights its innovative approach to blockchain scalability and security, making it a significant player in the DeFi ecosystem.