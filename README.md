# Performant Cosmos R&D Utilizing ABCI++
<br />

## 1. Reasoning

<br />

### Status of Cosmos Framework

After born of Tendermint and Cosmos-SDK framework, there has been improvement in features. Most notable improvement is IBC(Inter-Blockchain Communication) protocol, allowing cross-chain interaction among Cosmos chains. However, the scalability and performance haven’t significantly improved since 2019.

Outside Cosmos, there has been continuous improvement of dPoS blockchain technology to achieve better scalability and performance, such as Solana, Avalanche, Aptos and more. In Cosmos, introduction of ABCI++ opened up various R&D possibilities to optimize consensus, transaction handling and state transition processes.

<br />

### Cosmos as Standard Blockchain Technology

Unfortunately, those diversified R&D efforts are not benefitting whole Cosmos Ecosystem, including Cosmos Hub. Teams like Binance Chain, Sei, dydx, Celestia, Hyperliquid are forking or referencing Tendermint/CometBFT and Cosmos-SDK for their own usecases but it does not result in improvement of the standard Cosmos technology. This result in the situation where the standard Cosmos technology stays behind other recent technologies, ultimately threatening the position of Tendermint/CometBFT and Cosmos-SDK as the performant blockchain technology stack especially in mass adoption scenario.

From Cosmos Hub perspective, its main revenue model is becoming ICS(Inter-Chain Security) which requires performant Cosmos tech stack to persuade consumer chains to be part of the Cosmos Hub ICS ecosystem. Considering successful ICS model rely on the many success of ICS zones with significant userbase and activities, the performant tech stack is one of the most important condition for the growth of Hub ICS ecosystem.

<br />

## 2. How

<br />

### Recent Blockchain Technology to Cosmos Tech Stack

Therefore, we need timely and continuous efforts to keep up with recent technology development in the entire space for the Cosmos tech stack to survive in mass adoption phase of the blockchain cycle. In mass adoption phase, there will be many mega-applications with millions of userbase who will need a blockchain tech stack which can handle such large community. Because R&D takes long time to have a secure production level codebase, we need steady and continuous effort invested for such R&D. Relying on generous upstream PRs from independent blockchain teams are not a competent strategy.

<br />

### Separate Repository for Performance R&D

Even though we will do our best to have maximized compatibility with existing users, these improvements on Tendermint/CometBFT and Cosmos-SDK might cause some compatibility issue on existing chains to adopt with, because of significant rebase work caused from breaking changes in the structure of the tech stack, followed by potential security risk factors. 

Hence, the performance R&D should not be limited by such conservative environment of current main branch whose main priority is security and stability. Therefore, we suggest a separate repository to accelerate R&D capability without any practical barriers from existing technically conservative approach, which allows maximized freedom to explorer various design options.

<br />

### Expected Roadmap

The first proposal only includes the research work necessary to explore various design options to be compared. This is because many part of performance improvement directions are not obvious with different methodologies existing. We need to figure out top design options which have most significant performance impact, least compatibility issues and security assumptions, and less complexity to implement.

After completion of our proposed research, a follow-up project can be proposed to implement most reasonable design options as PoC so that we can prove the practicality of performant Cosmos tech stack without hurting compatibility for IBC connections with existing Cosmos ecosystem. Production level codebase project can be followed after PoC step for practically usable tech stack implementation.

<br />

## 3. Funding

<br />

**1) Research : 2.5 devs * 3 months * $20k = $150k**

- Research multiple improvement in Tendermint/CometBFT/Cosmos-SDK from Sei, BNB and some other chains and suggest the most useful directions for performant Cosmos tech stack implementation.

<br />

**2) PR on Vesting Module for Cancellation by Governance : 0.5 dev * 1 month * $20k = $10k**

- Adding vesting cancellation via governance feature to existing vesting module
- Context : This work is added to allow more flexible community fund or subDAO spending by introducing vesting cancellation by governance or multi-sig.

<br />

**Total : $160k**
