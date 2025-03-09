# What Is GAS? Ethereum HIGH Transaction Fees Explained

*Upload Date: 20210220*

*Source: [https://www.youtube.com/watch?v=Yh8cHUB-KoU](https://www.youtube.com/watch?v=Yh8cHUB-KoU)*

# Understanding Ethereum Gas and High Transaction Fees

## Introduction to Gas

Gas is a unit used in the Ethereum blockchain to measure the computational effort required to execute specific operations. It is a crucial concept in Ethereum as it helps in quantifying the cost of executing transactions and smart contracts. The gas mechanism ensures that users pay for the computational resources they use, preventing the network from being overwhelmed by malicious or inefficient code.

### Why Gas Exists

The primary reason for the existence of gas is to prevent the halting problem, which is a theoretical issue in computer science where it's impossible to determine if a program will run indefinitely. By requiring gas for each operation, Ethereum ensures that no single transaction can consume an infinite amount of computational resources, thus preventing the network from grinding to a halt.

## Gas Cost and Transaction Fees

### Gas Cost Calculation

The gas cost for a transaction is calculated by multiplying the gas limit (the maximum amount of gas the user is willing to spend on the transaction) by the gas price (the cost of one unit of gas in ether). The gas price is set by the user and reflects the urgency of the transaction. Higher gas prices incentivize miners to prioritize the transaction, leading to faster confirmation times.

### Transaction Fee

The transaction fee is the product of the gas used and the gas price. It is paid by the user to the miner who includes the transaction in a block. This fee compensates the miner for the computational work and the risk of including the transaction.

## Factors Influencing Gas Prices

### Network Activity

The gas price is influenced by the network activity. During periods of high activity, the demand for block space increases, driving up gas prices as users compete to have their transactions included in the next block. Conversely, during low activity periods, gas prices tend to be lower.

### Urgency of Transactions

Users who want their transactions to be confirmed quickly may set a higher gas price, making it more attractive for miners to include their transactions in the next block. This creates a market-driven mechanism for determining gas prices.

## Solutions to High Gas Prices

### Layer 2 Scaling Solutions

Layer 2 scaling solutions are built on top of the Ethereum mainnet (Layer 1) and aim to increase the network's transaction throughput and reduce costs. Examples include:

- **Loopring**: A decentralized exchange built on Layer 2 that allows for cheaper and faster transactions.
- **Matic (Polygon)**: A Layer 2 solution that has gained significant traction, with over $200 million in total value locked.
- **Optimism**: A Layer 2 solution based on optimistic rollups, which is being rolled out and aims to further reduce transaction costs.

### Ethereum 2.0 (Eth2)

Ethereum 2.0 introduces sharding and proof of stake, which are expected to significantly increase the network's scalability and reduce transaction costs in the long run.

### EIP-1559

EIP-1559 is a proposal that aims to optimize the fee model by smoothing out gas price spikes and limiting the number of overpaid transactions. It makes transaction fees more predictable and could be implemented in early 2021.

### Other Tricks

- **Timing**: Users can wait for periods of lower network activity to send transactions at lower gas prices.
- **Gas Estimation Tools**: Using tools like EthGasStation.info to estimate gas costs.
- **QI Tokens**: Leveraging mechanisms like QI tokens, which can reduce the total gas spent in a transaction by burning these tokens alongside the primary operation.

## Alternative Chains

Other blockchain networks have emerged as alternatives to Ethereum, offering lower transaction fees and faster confirmation times. However, some of these chains may not be fully decentralized or permissionless, creating a "fake" decentralized ecosystem that is not much different from using a centralized exchange.

## Conclusion

High transaction fees on Ethereum are a result of the network's popularity and the high demand for block space. While this presents challenges, various solutions such as Layer 2 scaling, Ethereum 2.0, and EIP-1559 are being developed and implemented to address these issues. Users can also employ strategies like timing their transactions and using gas estimation tools to manage costs effectively.