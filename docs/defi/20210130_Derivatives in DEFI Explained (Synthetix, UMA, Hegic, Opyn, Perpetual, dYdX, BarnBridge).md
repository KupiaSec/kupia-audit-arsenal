# Derivatives in DEFI Explained (Synthetix, UMA, Hegic, Opyn, Perpetual, dYdX, BarnBridge)

*Upload Date: 20210130*

*Source: [https://www.youtube.com/watch?v=QxoqPZRw9y4](https://www.youtube.com/watch?v=QxoqPZRw9y4)*

# Derivatives in DeFi: A Comprehensive Overview of Protocols and Concepts

Derivatives play a crucial role in mature financial systems. In DeFi (Decentralized Finance), derivatives derive their value from an underlying financial asset, such as stocks, bonds, commodities, currencies, or cryptocurrencies. Common types of derivatives include forwards, futures, options, and swaps.

## Key Use Cases for DeFi Derivatives

Derivatives serve two primary purposes:

1.  **Hedging:** managing financial risks. It helps DeFi user to avoid potential losses. The Farmer example shows how farmers can using derivatives (wheat futures contracts) in order to avoid loses. The other example shows how DeFi users use hedging to offset a potential loss linked to yield farming tokens.
2.  **Speculation:** Speculation drives a significant amount of trading volume due to derivatives offering easy exposure to specific assets that might be otherwise hard to access and easy access to leverage.

## Prominent DeFi Derivatives Protocols

Here's an overview of popular DeFi derivatives protocol.

### 1. Synthetix

Synthetix enables the creation of synthetic assets (Synths) that track the price of underlying assets. It currently supports synthetic fiat currencies, cryptocurrencies, and commodities.

*   **Mechanism**:  Synthetix employs a **pooled counterparty** model also known as deadpool. Users need to provide collateral in the form of SNX tokens (Synthetix Network Token) to mint synthetic assets.
*   **Collateralization**:  It uses over-collateralization (currently at 500%). For every 500 USD worth of SNX locked, only 100 USD worth of synthetic assets can be issued.
*   **Layer 2 Migration**: Synthetix is actively working on migrating to Layer 2 solutions to lower gas fees and improve scalability. Quenta, dHedge, and Paraswerb are example trading platforms.
*   **Total Value Locked (TVL)**: Approximately $1.8 billion.

### 2. UMA (Universal Market Access)

UMA is another protocol facilitating the creation of synthetic assets. However, it uses a different mechanism.

*   **Priceless Derivatives:** UMA enables the creation of "priceless" derivatives, meaning it doesn't rely on price oracles in the optimistic scenario. Instead, it depends on liquidators who are financially incentivized to identify & liquidate improperly collateralized positions.
*   **Innovation Tailwind:** Allows adding a very long tail of synthetic assets that wouldn't have a reliable price feed.
*   **Total Value Locked (TVL)**: Over $63 million.

### 3. Hegic

Hegic is a relatively new DeFi project focused on options trading in a non-custodial and permissionless fashion.

*   **Options**:  Users can buy put or call options on ETH (Ether) and WBTC (Wrapped Bitcoin). Others can become liquidity providers and sell these options
*   **Options Style**: Hegic uses American-style options, which can be exercised at any time before expiration, unlike European-style options that can only be exercised at expiration.

### 4. Opyn

Open, launched in early 2020, is a protocol for trading options.

*   **Focus**:  Started by offering Ether downside & upside protection, allowing users to hedge against ETH price movements.
*   **v2 Upgrade**: Offers European cash-settled options that auto-exercise upon expiry.

### 5. Perpetual Protocol

Perpetual Protocol is a new entrant in the decentralized derivatives space, focused on perpetual contracts.

*   **Perpetual Contracts**: It facilitates perpetual contracts trading. A perpetual contract is a popular trading product used used on centralized platforms such as BitMEX and Binance.
*   **Settlement**: Trades are funded and settled in USDC (a stablecoin).
*   **Layer 2 Solution**:  Perpetual Protocol uses xDAI chain- a Layer 2 scaling solution- to process trades, resulting in low gas fees.

### 6. dYdX

dYdX is a decentralized exchange offering spot, margin, and perpetual trading.

*   **Architecture**: It combines non-custodial on-chain settlement with an off-chain, low-latency matching engine and order books.
*   **Scaling**: New perpetual contracts product is launching on Layer 2, powered by StarkWare's zk-rollups.

### 7. BarnBridge

BarnBridge is a risk-tokenizing protocol.

*   **Focus:** It offers hedging yield sensitivity & price volatility, using debt-based derivatives and smart alpha bonds (covering market price exposure risk) as well as tranche volatility derivatives.
*   **Mechanism:** It accesses deadpools from other DeFi protocols to create assets with different risk-return characteristics.

## Important Considerations

Interacting with new DeFi protocols carries inherent risks. It's crucial to:

*   **Do Your Own Research (DYOR)**: Always conduct thorough due diligence. Be aware that many of these projects is still in beta or early stages.