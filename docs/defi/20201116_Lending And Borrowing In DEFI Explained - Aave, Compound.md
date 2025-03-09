# Lending And Borrowing In DEFI Explained - Aave, Compound

*Upload Date: 20201116*

*Source: [https://www.youtube.com/watch?v=aTp9er6S73M](https://www.youtube.com/watch?v=aTp9er6S73M)*


# Lending and Borrowing in DeFi: A Deep Dive into Aave and Compound

Lending and borrowing are fundamental components of any financial system, and DeFi is no exception. This article explains how lending and borrowing work in the decentralized finance (DeFi) space, focusing on popular protocols like Aave and Compound.

## What is DeFi Lending & Borrowing?

DeFi lending & borrowing operates on the concept that lenders (depositors) provide funds to borrowers in exchange for interest payments. Unlike traditional finance, DeFi facilitates this process in a decentralized and permissionless manner, allowing users worldwide to participate without intermediaries.

## DeFi vs. CeFi Lending

**CeFi (Centralized Finance)** platforms operate similarly to banks, taking custody of deposited assets and lending them out. While convenient, this approach suffers from centralization risks such as hacks and negligence.  Furthermore, Cefi Lending goes against the fundamental value propositions of cryptocurrency:  self-custody.

**DeFi lending** enables users to become lenders or borrowers in a completely decentralized, permissionless manner while retaining *custody* over their coins.  DeFi Lending is based on smart contracts that run on open blockchains (predominantly Ethereum), making it accessible to everyone without the need for personal details or trusting a third party.

## How Aave and Compound Work

Aave and Compound are two leading DeFi lending protocols. Both create money markets for specific tokens, such as Ether (ETH), stablecoins like DAI and USDC, and other tokens. Users become lenders by supplying their tokens to a particular money market, earning interest based on the current supply API (Annual Percentage Yield).

### Mechanics in Detail

1.  **Token Supply:** Lenders deposit their tokens into a smart contract.
2.  **cTokens/aTokens:** In exchange, the lender receives cTokens (Compound) or aTokens (Aave) representing their deposit and accrued interest. These tokens can be redeemed for the underlying assets.
3.  **Borrowing:** Other users can borrow these supplied tokens by providing collateral.
4.  **Interest Rate Determination:** Interest rates for both lenders and borrowers are algorithmically determined based on the ratio of supplied and borrowed tokens within a specific market. Typically, the borrower API is higher than the supply API
5.  **Variable Interest Rates:** Aave offers both variable and stable borrow APRs, while Compound offers variable rates by default.

## Collateralization

Most DeFi loans are *collateralized*. To borrow funds, a user must supply tokens as collateral, which must be worth more than the actual loan amount.

### Why Collateralize?

Reasons for using DeFi lending even with existing assets:

*   **Avoiding Token Sales**:  Users might need funds but want to avoid selling their crypto holdings and incurring potential capital gains taxes.
*   **Increased Leverage:** Borrowed funds can be used to increase leverage in a specific position.
*   **Unexpected Expenses**: A user wants fund to cover expenses when they don't wnat to sell the coins.

### Collateral Factor

The amount that can be borrowed depends on two main factors:

1.  The quantity of tokens available to be borrowed in each market. The higher, the better.
2.  The collateralisation factor of the supplied tokens.

Collateral factor determines how much can be borrowed based on the quality of the collateral. For example, DAI and ETH might have a collateral factor of 75% on Compound, meaning that up to 75% of the value of the supplied DAI or ETH can be used to borrow other tokens.

### Liquidation

If the value of the collateral falls below a required level, the user's collateral will be liquidated to repay the borrowed amount and associated interest.

## Key Differences: Variable vs. Stable Rates + Flash Loans

While both protocols offer variable supply and borrow APIs, Aave also provides stable *borrow* APIs. This stable rate offers short-term predictability, though it can change over the long term to accommodate market conditions.

Aave also offers flash loans, enabling users to borrow funds with no upfront collateral for a very short period for *advanced* and *atomic transactions* in a single Ethereum transaction (single block).

## Practical Example: Depositing ETH and Earning Interest on Compound

Consider a user depositing 10 ETH into Compound. Upon deposit, the protocol issues cTokens (cETH) to the user. The amount of cETH received depends on the current exchange rate between cETH and ETH, for instance, an exchange rate of 0.02 would result into the lender receiving 500cETH. As other people need money after the tokens are deposited, as time goes by, there's another block and now the exchage rate has been adjusted to `0.021`.

Over time, with each Ethereum block, the exchange rate between cTokens and the underlying assets increases, reflecting accrued interest. Let's say, after a month, a block has been created and the user decides to reedem to its ETH in compound, now the resulting amount would be now around `10.0165`. In that case, the lender receives the increased underlying asset amount, which is interest.

## Risks to note

*The following are risks when using Defi Lending:*

*   Smart Contract Risks: Defi Depends on smart contract, hence these smart contract needs to be audited or else a user could lose money
*   Volatility APRs
*   Liquidations

Understanding Defi lending and its protocols is one way to enter the decentralized financial system.
