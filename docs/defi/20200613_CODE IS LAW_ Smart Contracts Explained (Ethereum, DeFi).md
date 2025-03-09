# CODE IS LAW? Smart Contracts Explained (Ethereum, DeFi)

*Upload Date: 20200613*

*Source: [https://www.youtube.com/watch?v=pWGLtjG-F5c](https://www.youtube.com/watch?v=pWGLtjG-F5c)*

# Code is Law? Understanding Smart Contracts on Ethereum and DeFi

## Introduction: The Rise of "Code is Law"

The expression "Code is Law" reflects a futuristic trend where technology enforces rules, potentially reducing the need for lawyers and creating a fully automated world. This concept becomes more tangible with the continuous development of smart contracts. So lets explore smart contracts, their functionalities, advantages, and disadvantages, how these are used, and the challenges involved.

## What is a Smart Contract?

A smart contract is a piece of code that can be executed automatically on a blockchain in a deterministic way. This means that the same input will always produce the same output, ensuring predictability and reliability.

*   **Deterministic Execution:**  The outcome of a smart contract execution is always predictable, given the same initial conditions.
*   **Blockchain Storage and Execution:** Smart contracts are stored and executed on a blockchain, making them trustless and secure.
*   **Capabilities:** Smart contracts can receive, store, and send funds, as well as call other smart contracts.
*   **If-Then Semantics:** Smart contracts operate based on "if-then" logic, making them relatively easy to program.
*   **Goal:** is to remove the human factor from decision-making, which is often error-prone and unreliable in traditional contracts.

## Smart Contracts vs. Traditional Contracts: A Vending Machine Analogy

A vending machine serves as a good analogy for understanding smart contracts. A vending machine is programmed to allow certain actions and state transitions based on input.

*   **Deterministic Operation:**  A vending machine works in a fully deterministic way. For example, if you insert enough payment for a product, the machine will dispense it according to its programming.
*   **Limited Logic:** The machine's actions are predefined based on which coins are available and which it is programmed to accept.
*   **Smart Contract Equivalence:**  Similar to a vending machine, a smart contract relies on blockchain information or external data sources (oracles, like Chainlink) to execute its code.

## Smart Contracts: Benefits Over Traditional Contracts
Here are some reasons why smart contracts have benefits compared to traditional contracts.

*   **Trustlessness:** No need to trust a third party, contracts are automated through code
*   **Holding Funds:** Smart contracts hold funds within themselves, which is not practical for traditional contracts.
*   **Speed:** Transactions can be completed seconds after initial criteria are met.
*   **Cost-Effective:** Eliminates intermediary costs like lawyer fees and potential insurance costs.
*   **Eliminates arbitration and Enforcement Costs:** These are automatically executed with smart contracts.
*   **Reusability:** Can be used to perform a single task for many use cases.

### Example: Token Swapping with Alice and Bob

In a traditional finance setting, Alice and Bob would need to trust an intermediary to execute a token swap. To mitigate this, there is an escrow contract with a third party collected funds from Alice and Bob to release appropriate funds, that could be lost. The alternative with smart contracts would be more secured.
*   **Smart Contract Solution:**  A smart contract can automate the token swap in a trustless manner.  Alice and Bob can deposit tokens into the contract, and when the required number of tokens are deposited, the contract automatically swaps the tokens between them.
*	**Ethereum and Solidity:** In Ethereum, smart contracts can be written by solidity.

## Smart Contracts on Ethereum
All contracts written for Etherium are immutable when deployed.

*   **Decentralization:** No single machine controls the contract; all nodes on the Ethereum network store the same contract and its state.
*   **Immutability:** Once deployed, smart contracts cannot be modified, creating certain risks that must be carefully considered.
*   **General-Purpose Platform:** Ethereum is a popular platform for smart contracts, but faces stiff competition like Cardano , Tezos and so on.
*   **Growing use of smart contracts:** Has a growing number from use cases for supply chains, crowdfunding and basic building blocks for decentralized applications (dApps)

## Use Cases for Smart Contracts

Smart contracts find applications in various sectors:
### 1. DeFi (Decentralized Finance)
Using decentralized smart contracts, financial concepts can be reproduced without central control:
1.  **Stablecoins:** Smart contracts are used together with some incentives to create stable coin, whose goal is to have a U.S. dollar paired value ratio.
2.  **Automated  Liquidity Provisioning:** Smart contracts are used to swap tokens in fully permissionless fashion.
#### Other than that, some famous protocols are Uni Swap and Kyber Network
### 2. Supply Chain Transparency
Blockchain makes it more transparent and secure to track what part of the supply chain and with protocols likes OriginTrail, the origin and trace of goods.

### 3. Crowdfunding
A lot of initial coin offers (ICOs), where you are unlocking code to release funds after verified community approvals.

### 4. Ride-Sharing
The most futuristic use case, where there are no intermediaries necessary.

## Challenges and Risks

Despite their potential, smart contracts are not without challenges:
**1. Software Bugs:**
*   **The DAO Hack:**  A prime example of a bug in a smart contract was the DAO hack, resulting in millions of dollars worth of Ether being lost.
*   **Formal Verification:** The community now focuses on security audits and formal verification methods.

**2. Protocol Changes:**
*   **Upgrades:** Even with bug-free, audited contracts, upgrades to the underlying blockchain platform can cause unexpected behavior. So you will have to have real-world issues can be visible.
*   **Oracle Services:** Is a true solution to the chain but, this will always need to be trusted.

## So....Can Code Replace Lawyers?

Lawyers can not exactly be replaced as we have regulatory and tax challenges, although with valuable knowledge, and translated into code, maybe.

## Conclusion: Opportunities and Challenges Ahead

Smart contracts offer automation, deterministic results, trustless interactions, and cost efficiency. However, they also present challenges, including software bugs, protocol changes, and regulatory uncertainties. Nonetheless, continued progress in this field promises a future where digital agreements are more reliable and efficient.