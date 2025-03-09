# How Does AMPLEFORTH Work? DEFI Explained

*Upload Date: 20200727*

*Source: [https://www.youtube.com/watch?v=e-8yjmsshFg](https://www.youtube.com/watch?v=e-8yjmsshFg)*


# Ampleforth Explained: How Does it Work?

Ampleforth (AMPL) is a cryptocurrency designed with an elastic supply, aiming for price stability and diversification within crypto portfolios. This article explains the mechanics of Ampleforth in detail.

## What is Ampleforth?

Ampleforth is a cryptocurrency that adjusts its supply algorithmically in response to price fluctuations. This unique feature makes it different from cryptocurrencies like Bitcoin, which have a fixed supply.

## Elastic Supply: The Core Feature
The supply of AMPLtokens changes daily based on market demand. This differs from fiat currencies like the US dollar, where central banks can decide to print or remove money, and cryptocurrencies like Bitcoin, where the supply is fixed.

## Non-Dilutive Ownership

A key characteristic of Ampleforth is that it is *non-dilutive*. This means that even though the number of AMPL tokens a user holds can change daily, the proportion of the total supply that they own remains constant.  This is achieved through a mechanism called rebase.

## Elastic Supply and its Impact
Elastic supply in traditional currencies (like the USD) allows for printing or removing money depending on demand. The Federal Reserve, for example, prints more money to accommodate increased demand. However, this can lead to **dilution**.

Bitcoin, on the other hand, has a fixed supply. To accommodate an increase in demand, the price of Bitcoin must increase. While it is **non-dilutive**, the constant increasing price can be problematic when it comes to pricing of services, contracts or debt.

## Ampleforth's Solution: Elastic and Non-Dilutive
Ampleforth aims to combine the best aspects of both: an elastic supply *and* non-dilutive ownership.  While the numbe of your tokens can change, you will always own the same total supply of the token.

## Ampleforth States: Expansion, Contraction, and Equilibrium

The Ampleforth protocol operates in three states:

*   **Expansion:** The supply of AMPL tokens is proportionally increased across all wallets.

*   **Contraction:** The supply of AMPL tokens is proportionally decreased across all wallets. This is the exact opposite of Expansion.

*   **Equilibrium:** The algorithm doesn't change the supply and where there's no need to do anything.

## The Role of Price Oracles

Price oracles are essential for Ampleforth to function. They provide external price data to the smart contracts. These oracles serve two main functions:

1.  **Current Exchange Rate:** Provide the current exchange rate of AMPL to USD.
2.  **Consumer Price Index (CPI):** Provide a consumer price index value. This establishes the **target price** for one AMPL token, which is currently set to the 2019 purchasing power of the US dollar (approximately $1.009 USD).

This target price is a very important part of The Ampleforth Protocol. Because The Ampleforth Protocol tries to aim for that target price.

## The Rebase Function

Ampleforth utilizes a function to automatically control the Expansion or Contraction, called the rebase function. It's called every day at 2 AM UTC time , and uses the Price Oracles that were defined earlier to achieve the goal of the rebase function.

### Stateless Design

The rebase function is *stateless*, so that the algorithm recomputes the potential supply change every day based on the latest information from the price oracles. It doesn't have any "memory" of the previous function.

## Implementation: Smart Contracts on Ethereum

The Ampleforth protocol is implemented as smart contracts deployed on the Ethereum blockchain. The AMPL token implements the ERC-20 interface, making it compatible with decentralized exchanges (DEXes) such as Uniswap.

## Blockchain Agnostic
Ampleforth is *blockchain agnostic* and can simultaneously exist on multiple platforms.

## Goals of Ampleforth

*   **Short Term:** Diversify Cryptocurrency portfolios by being less correlated to Bitcoin's price than other cryptocurrencies.
*   **Medium Term:** Serve as collateral in DeFi protocols.
*   **Long Term:** To create an alternative to central bank money that is adaptable to shocks. It wants to incentive more unchain liquidity; this is why an inceptive called Geyser was created.

## Geyser: Incentivizing Liquidity
Ampleforth created an incentive for liquidity providers using Geyser. Rewards the liquidity providers in UNI and LP tokens. Check the document description box for more information.

## Key Takeaways

*   Always look at the number of the tokens in addition to the price, to monitor the performance.

*   Ampleforth is a monetary experiment on the functionality of being used as money in the future.
