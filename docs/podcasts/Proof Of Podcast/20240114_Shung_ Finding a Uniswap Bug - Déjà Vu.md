# Shung: Finding a Uniswap Bug - Déjà Vu

*Upload Date: 20240114*

*Source: [https://www.youtube.com/watch?v=680Ljx0xtmU](https://www.youtube.com/watch?v=680Ljx0xtmU)*


## Shung: Finding a Uniswap Bug - Déjà Vu - Summary

This document summarizes a Youtube interview with Shung, a security researcher, about his experiences in the DeFi space and specifically his finding of a bug in Uniswap V3.

**Part 1: Introduction and Background**

*Q: Please introduce yourself.*

*A: Shung introduces himself as an independent security researcher, currently working with Kebab Sack. He previously worked at Pangolin Exchange on Avalanche, contributing to staking functionalities.*

*Q: What do you make of the recent Avax activity?*

*A: He notes the recent "heat" and hype around Avalanche Community and the importance of responsible decision making amid the hype.*

*Q: How did you get into crypto?*

*A: He says he was initially drawn to crypto through libertarian values, aspiring to be his own bank.  His entry point was Avalanche which gives it a special place in his heart and appreciated that each new fork was an opportunity to learn the existing code.*

**Part 2: Path to Security Research**

*Q: Why Avalanche?*

*A: He was initially drawn to the tokenomics but quickly transitioned to the technology.  He started following the project after reading their whitepaper and was engaged when the Avalanche Bridge was deployed.*

*Q: Can you expand on your technical growth?*

*A: It began as a user of Avalanche and then TXS. As the project developed, he made crypto friends. All his learning experience led him to becoming a Solidity expert.*

*Q: How can someone get to your coding level, with that gradual learning process?*

*A: Need good standards, making everything immutable aligning with blockchain philosophy and gas optimization.*

**Part 3: The Uniswap V3 Bug and Report Style**

*Q: Why do you include humor in your bug reports?*
*A: You need to have some standards. To make things immutable for example which aligns with the philosophy of the blockchain. He says it will make the experience for other learners better*.

*Q: How did you get with Bengal index?*
*A: He has libertarian values as well.*

*Q: How did Bengal index capture you?*

*A: NFT project got his parents involved with drawing most of the traits in that project.  Then, through an internship, he was starting to become more interested in development. He didn't know Solidity code, copy and pasting but this way he learned the APIs works*.

*Q: How did you get to Pangolin?*

*A: There was an intern position. After doing that position, they invited him to join. The top was Justin!*

*Q: How did Pangolin led into the independent auditing career?*

*A: There were experiences with bugs. Then a new job offered that!*

*Q: How did his journey to Spearbit begin*:

*A: A guy from Turkey went to a blockchain event and Shung spoke with him and asked Shah's parents*

*Q: So can can u tell us a uniswap V3 bug?*

*A: The code will pass all codes and unit test. Still there was the bug but most reports are extremely hard*

*Q: So can we have a colorful report like yours?*
*A: There is 60 70% luck, it was a big part of it*

*Q: How to avoid it for new auditing beginners?*
*A: Do not be irresponsible, it is a meme and hype, make sure to have the code audited*

*Q: Talk more detail for these Uniswap V3 bug*

*A: Basically his code was sent to spear bits, where Bhauhum found a uniswap V3 bug*

The bug in Uniswap V3 was related to the settlement design and the use of a logarithm function. A flaw in how this logarithm function handled numbers with decimal points would cause the incorrect return of a number

This "luck" leaded him to that bug due that there was that issue.

**Part 4: Advice and Future of Audited Security**

*Q: What would you suggest for building that auditing or security career?*

*A: Take it slowly and always read other people's. Standards are very very important for improving your learning. Gas Optimization.
To have something immutable! That aligns with a blockchain.*

*Q: How should people test, code, approach building in web3?*
*A: Rewrites stuff based on his standards. Get everything optimized*

*Q: How can people work with you?*
*A: He had cryptocurrency friends.*

*Q: What is your opinion to Web Free if the security tools have AI improving them more*

*A: Web free security will not get better. Learn security and has that experience from spearbit and so, you can have more control by getting crypto friends to help*

*Q: Did you think they would be able to put a stop to that type of hack*
*A: No, all developer must need to know the security and be a expert on it. *

Finally, Shung encourages newcomers to learn, share, and contribute and learn what they are building. He emphasizes that security is everyone's responsibility in the web3 space.
