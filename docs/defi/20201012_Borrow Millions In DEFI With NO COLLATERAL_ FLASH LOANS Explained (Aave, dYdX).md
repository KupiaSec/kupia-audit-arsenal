# Borrow Millions In DEFI With NO COLLATERAL? FLASH LOANS Explained (Aave, dYdX)

*Upload Date: 20201012*

*Source: [https://www.youtube.com/watch?v=mCJUhnXQ76s](https://www.youtube.com/watch?v=mCJUhnXQ76s)*

# Flash Loans Explained: Borrow Millions in DeFi with No Collateral

Flash loans are a revolutionary DeFi feature that allows users to borrow assets without providing any upfront collateral. These loans must be borrowed and repaid within the *same* blockchain transaction. This article dives into the mechanics, use cases, and risks associated with flash loans, primarily focusing on implementations by Aave and dYdX.

## What are Flash Loans?

A flash loan is a type of uncollateralized lending facilitated by smart contracts. Key characteristics:

*   **No Collateral Required:** Borrowers don't need to lock in any assets as collateral.
*   **Single Transaction:** The borrowed funds along with any fees, must be repaid within the same blockchain transaction.
*   **Atomic Transaction**: It means if the transactions fail, all steps are rolled back.
*   **Smart Contract Driven:** Flash loans are enabled by specific smart contracts acting as lending pools.

Flash loans were popularized by Aave and dYdX, although initially introduced by Marble protocol and serve as building blocks for complex DeFi strategies.

## Transactions on the Blockchain

Understanding transactions on a blockchain is crucial to grasping flash loans. A transaction represents a set of operations executed atomically – all steps succeed, or all steps are rolled back, ensuring data consistency.

**Analogy: Database Transaction:**

Consider a database transaction that transfers funds from Alice to Bob. The transaction consists of two update statements:

1.  Subtract funds from Alice's balance.
2.  Add funds to Bob's balance.

If the second statement fails, perhaps due to an invalid Bob's ID, you don't want Alice's balance to be updated without Bob's balance. Wrapping the statements within a transaction (e.g., using `BEGIN` and `COMMIT` in SQL) ensures that either both updates occur, or none do.

**Ethereum Transactions:**

Similarly, Ethereum transactions encompass multiple steps, such as sending tokens, interacting with smart contracts, and executing DeFi operations (e.g., supplying ETH and borrowing DAI on Compound, swapping DAI for USDC on Curve, providing liquidity on Uniswap). If any step within a transaction fails, the *entire* transaction is reverted, and none of the individual steps take place. Note: Gas fees are still paid for failed transaction attempts.

The gas cost limit of each block bound the number of steps of a single transaction.

## Mechanics of Flash Loans

1.  **Identifying a Flash Loan Provider:** Projects like Aave and dYdX provide smart contracts that enable flash loans.
2.  **Borrowing:** A user borrows assets from a designated pool with the condition of repayment within the *same* transaction.
3.  **Usage and Repayment:** The borrowed funds can be used for arbitrary actions, provided that the loan is repaid, along with applicable fees, before the transaction concludes. Aave, for instance, charges a fixed fee of 0.09% of the borrowed amount. The protocol distributes the fee amongst depositors who provided the fund and the integrators who facilitated the use of Aave's flash loan API. Also, a part of that fee is swapped to other tokens and burned.
4.  **Risk Mitigation:** Repayment within the same transaction eliminates the risk of default because if the loan with fees can't be repaid for any reason, the smart contract will revert the transaction meaning no changes will take place.

*Note: Risk comes because of smart contact and platform risk.*

## Use Cases for Flash Loans

Flash loans enable various sophisticated DeFi strategies:

1.  **Arbitrage:** Flash loans magnify profits from price discrepancies across different exchanges.

    *   **Example:**
        *   DAI/USDC pair: 1 DAI = 1 USDC on Curve, but 0.99 DAI = 1 USDC on Uniswap.
        *   **Strategy:**
            1.  Borrow 100,000 DAI via flash loan from Aave.
            2.  Swap 100,000 DAI for USDC on Uniswap (receiving ~101,010 USDC).
            3.  Swap 101,010 USDC for DAI on Curve (receiving ~101,010 DAI).
            4.  Repay 100,000 DAI + 0.09% fee (90 DAI) to Aave.
            5.  Profit: 920 DAI

    *   **Considerations:** Network fees, price slippage (impact of order size on price), front-running (other bots spotting and executing the same arbitrage).

2.  **Collateral Swaps:**  Change collateral on lending platforms without closing existing positions.

    *   **Example:** Swap ETH collateral for BAT on Compound.

        1.  Take a flash loan in DAI to cover the DAI borrowed on Compound.
        2.  Repay the Compound loan with the flash loan DAI.
        3.  Withdraw the ETH collateral.
        4.  Swap the ETH for BAT on Uniswap.
        5.  Supply BAT as collateral on Compound.
        6.  Borrow DAI against the BAT collateral.
        7.  Repay flash loan with borrowed DAI plus fees.

3.  **Self-Liquidation:**  Prevent liquidation during a market downturn.

    *   **Example:** Prevent liquidation of your ETH-backed DAI loan on Compound.

        1.  The ETH price is dropping, approaching liquidation.
        2.  Take a flash loan of required DAI amount.
        3.  Repay the entire DAI loan and withdraw ETH collateral.
        4.  Swap just enough ETH for DAI to repay the flash loan + fees.
        5.  Keep the remaining ETH.

## Risks and Downsides of Flash Loans

While flash loans are powerful tools, they also present risks:

*   **Exploits and Attacks:** Flash loans have been used in DeFi hacks to manipulate prices or exploit vulnerabilities in smart contracts due to the large amount of asset with no collateral required.
*   **Smart Contract Risk:** As mentioned above, inherent smart contract vulnerability will always be the potential risk, so it can't be avoided completely.

It's essential to acknowledge and manage these risks when using flash loans. However, flash loan exploits do strengthen the DeFi ecosystem in the long run by uncovering vulnerabilities.

## Using Flash Loans Without Code

While many flash loan use cases involve coding smart contracts, some projects (e.g., Collateral Swap, Defi Saver, Furucombo) provide interfaces to leverage them without custom code.

## Conclusion

Flash loans are a major innovation in DeFi, enabling sophisticated strategies without requiring upfront collateral. However, understanding the mechanics, use cases, and associated risks is critical for responsible and profitable utilization. As the DeFi ecosystem evolves, new use cases for flash loans will likely emerge, further expanding their potential.