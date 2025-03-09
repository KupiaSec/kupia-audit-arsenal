# BANK RUN in DEFI - Lessons Learned From The Iron Finance Collapse

*Upload Date: 20210624*

*Source: [https://www.youtube.com/watch?v=HUokre-szPg](https://www.youtube.com/watch?v=HUokre-szPg)*

# BANK RUN IN DEFI: Lessons from the Iron Finance Collapse

## Introduction

The video discusses the collapse of Iron Finance, a decentralized finance (DeFi) project, and the lessons learned from this event. Iron Finance was a partially collateralized stablecoin protocol that aimed to revolutionize the DeFi space. However, it experienced a massive bank run, leading to significant financial losses for its users. This article summarizes the key points and insights from the video.

## Iron Finance Overview

Iron Finance was designed around three tokens: Iron (IRON), a partially collateralized stablecoin; Titan (TITAN), a governance token; and Steel (STEEL), a fully collateralized stablecoin. The protocol aimed to maintain the value of IRON at $1 through a mechanism involving minting and redeeming tokens.

### Mechanism of Minting and Redeeming

- **Minting IRON**: Users could mint IRON by providing a mix of collateral (USDC) and TITAN tokens. The collateral ratio was adjustable, starting at 100% and gradually decreasing.
- **Redeeming IRON**: Users could redeem IRON for collateral and TITAN tokens. If IRON was trading below $1, users could redeem it for more than $1 worth of collateral and TITAN, leading to arbitrage opportunities.

## The Collapse

### Initial Events

On June 16, 2021, the protocol noticed that some large liquidity providers (whales) started removing liquidity from the Iron-USDC pool and selling TITAN and IRON. This caused the IRON price to drop below $1, triggering a negative feedback loop.

### Negative Feedback Loop

As IRON's price dropped, users started redeeming IRON for collateral and TITAN, exacerbating the problem. The protocol's price oracle, which was used to determine the number of tokens to be minted or redeemed, began reporting stale prices. This led to a death spiral where users could redeem IRON for more collateral than its actual value.

### Bank Run

The situation exposed a major flaw in the protocol: it relied heavily on human coordination, especially in times of crisis. When the protocol stopped expanding and started contracting, users began to lose confidence, leading to a bank run.

## Lessons Learned

### Importance of Price Oracles

The failure highlighted the risks associated with price oracles. If an oracle reports stale prices or is manipulated, it can cause significant losses. Protocols should have robust mechanisms to handle compromised oracles.

### Liquidity Pool Risks

Providing liquidity in pools where one asset can drop to zero value is risky. Even if the second token doesn't lose value, users can still lose a significant portion of their capital.

### Celebrity Endorsements

Celebrity endorsements can be risky. While they can bring attention, they also come with great responsibility. High returns often come with high risks, and users should always do their own due diligence.

### Algorithmic Stablecoins

Building algorithmic stablecoins is challenging. It requires a deep understanding of market dynamics and careful consideration of potential risks. The numbers are not always on the side of the protocol, and second versions of failed protocols often do not achieve the same level of traction as the original.

## Conclusion

The collapse of Iron Finance serves as a cautionary tale for the DeFi community. It underscores the importance of robust protocol design, reliable price oracles, and thorough risk assessment. As the DeFi space continues to evolve, lessons from such events will be crucial in building more resilient and sustainable financial systems.