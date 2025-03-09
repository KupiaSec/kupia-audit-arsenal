# Can ETH Become DEFLATIONARY? EIP 1559 Explained

*Upload Date: 20201106*

*Source: [https://www.youtube.com/watch?v=MGemhK9t44Q](https://www.youtube.com/watch?v=MGemhK9t44Q)*


# Can ETH Become DEFLATIONARY? EIP 1559 Explained

Ethereum Improvement Proposals (EIPs) are formal requests for changes to the Ethereum network. EIP 1559, also known as the "fee burn" proposal, is notable for its potential implications on Ethereum's monetary policy and client applications.

## Current Fee Model and Its Inefficiencies
Currently, Ethereum uses a simple auction mechanism, also recognized as a first-price auction, for transaction fees. Users bid for block space by submitting a gas price they are willing to pay. Miners prioritize transactions with the highest gas prices, incentivizing users to overpay to ensure their transactions are included in the next block, which results in inefficiency and users overpaying transaction fees.

This system leads to several downsides on Ethereum:
*   **User inefficiency** Overpaying leads to economic inefficiency on Ethereum
*   **Wallet Issues**: Wallets often need to facilitate gas price adjustments, leading to a suboptimal user experience. Less experienced users might set default fees that become insufficient during gas spikes, resulting in long confirmation delays.&#x20;

## EIP 1559: A Proposed Solution

EIP 1559 aims to address these issues and achieve goals:
*   More predictable transaction fees.
*   Reduced delays in transaction confirmation.
*   Improved UX by automating fee bidding.
*   Creating a positive feedback loop between network activity and ETH supply.

### The Base Fee and Network Capacity
EIP 1559 introduces the idea of a "base fee," an automatic minimum price for transaction which represents a minimum price that transaction should pay.&#x20;
The base fee is adjusted per block based on network congestion:&#x20;
*   Incremented when the network is over 50% utilized
*   Decremented when utilization is below 50%.

The network capacity will be increased by max gas limit per block from 12.5 million to 25 million gas, doubling to the block size.&#x20;

The goal is an equilibrium at 50% network capacity.

### Miner Tips
A minor tip is included to incentivize miners to prioritize a transaction and is paid directly to them. Miner tips are very important for transactions with a quick confirmation.

### Example Scenario: EIP 1559 in Action

Under this model, during periods of high network activity, users would submit transactions with a higher miner tip.

A user can set a fee cap to limit what he will pay, in this case, that specific transaction will wait to be included into a block and be confirmed up the point that the price gets lower or equal than the fee cap.&#x20;

Therefore, under the new model the network user expereince gets better and better.&#x20;

### Fee Burning & ETH Supply

The base fee with EIP-1559 is always completely burned. Also, there is an important concept called fee cap, where the user gets to decide the maximum value, the whole process can go for.

Burning the base fee also sparks discussion regarding ETH potentially become deflationary, where miners only receive block rewards and miner tips, burning the base fee would reward the users of the network (and ETH holders in general) by making all Ether units more scarce.

The core of a "deflationary ETH" comes when the block reward plus miner tip is lower than the base fee burned!

However, burning ETH could lead to a loss of control of the long term monetary policy or economic security.

## Implications and Challenges: Concerns and Ethereum's Roadmap

EIP 1559 is designed to reduce the high volatility of the gas fees. In a way it seems like gas is more valuable as it gets more scarce.&#x20;

Wallets automatically setting new base fees would simplify the user experiences, however it is important that miners safely processes all transactions! ETH 2.0 and layer 2 will also be key for further fee reduction and better usage.&#x20;

Miners are reluctant to change due to lower profits. This proposal should belong to core eips which means it affect all the clients. The main challenges are overcomiming the DOS atacks to the networks, also miner could collude but there are ways to prevent it. This change also improves a lot Ethereum as a currency so that it's great.