# Performant Cosmos R&D Utilizing ABCI++

## **1. Reasoning**

### **Status of the Cosmos Framework**

Since the creation of the Tendermint and Cosmos SDK framework, several feature improvements have been made. The most notable enhancement is the introduction of the IBC (Inter-Blockchain Communication) protocol, enabling cross-chain interaction among Cosmos chains. These enhanced features have opened up possibilities for various application development. However, scalability and computational performance have not significantly improved since 2019.

Outside the Cosmos ecosystem, continuous improvements in dPoS blockchain technology have been made to achieve better scalability and performance. Examples include Solana, Avalanche, Aptos, and more.

Within the Cosmos ecosystem, the introduction of ABCI++ has provided various R&D opportunities to optimize consensus, transaction handling, and state transition processes. Sei-Protocol is an example of performance improvement utilizing ABCI++.

### **Cosmos as a Standard Blockchain Technology**

Despite R&D efforts by various projects, the development of the entire Cosmos ecosystem, including the Cosmos Hub, has not been fully realized. Projects such as Binance Chain, Sei, dydx, Celestia, and Hyperliquid are forking or referencing Tendermint/CometBFT and Cosmos-SDK for their own use cases. However, this has not resulted in the improvement of the standard Cosmos technology. As a result, standard Cosmos technology lags behind other recent technologies, jeopardizing the position of Tendermint/CometBFT and Cosmos-SDK as a performant blockchain technology stack, especially in mass adoption scenarios.

From the perspective of the Cosmos Hub, its main revenue model is Inter-Chain Security (ICS), which relies on a performant Cosmos tech stack to persuade consumer chains to become part of the Cosmos Hub ICS ecosystem. The success of the Hub ICS ecosystem depends on the success of ICS zones with significant user bases and activities. Therefore, a performant tech stack is crucial for growth.

## **2. How**

### **Bringing Recent Blockchain Technology to the Cosmos Tech Stack**

To thrive in the mass adoption phase of the blockchain cycle, the Cosmos tech stack needs continuous and timely efforts to keep up with recent technological developments. During this phase, there will be numerous mega-applications with millions of users that require a blockchain tech stack capable of handling such a large community. Since it takes time for R&D to yield a secure production-level codebase, steady and continuous investment in R&D is necessary. Depending solely on generous upstream pull requests from independent blockchain teams is not a sufficient strategy.

### **Separate Repository for Performance R&D**

While we will strive to maximize compatibility with existing users, the improvements made to Tendermint/CometBFT and Cosmos-SDK may introduce some compatibility issues for existing chains. Significant changes in the structure of the tech stack may require rebase work and pose potential security risks.

Therefore, we should not limit performance R&D to the conservative environment of the current main branch, which prioritizes security and stability. Instead, we suggest creating a separate repository to accelerate R&D capabilities without the practical barriers of existing technically conservative approaches. This will maximize the freedom to explore various design options.

### **Expected Roadmap**

The initial proposal includes research work to explore various design options and compare them. This is necessary because many aspects of performance improvement directions are not obvious and require different methodologies. The goal is to identify the top design options that have the most significant performance impact, the least compatibility issues, security assumptions, and less complexity to implement.

After completing the proposed research, we can propose a follow-up project to implement the most reasonable design options as a proof of concept (PoC). This will allow us to demonstrate the practicality of a performant Cosmos tech stack without compromising compatibility with IBC connections in the existing Cosmos ecosystem. Once the PoC step is complete, we can proceed with a production-level codebase project for a practical and usable tech stack implementation.

## 3. Funding

**1) Research : 2.5 devs * 3 months * $20k = $150k**

- Research multiple improvements in Tendermint/CometBFT/Cosmos-SDK from Sei, BNB and some other chains and suggest the most useful directions for performant Cosmos tech stack implementation.

**2) PR on Vesting Module for Cancellation by Governance : 0.5 dev * 1 month * $20k = $10k**

- Adding vesting cancellation via governance feature to existing vesting module
- Context : This work is added to allow more flexible community fund or subDAO spending by introducing vesting cancellation by governance or multi-sig.

**Total : $160k**
