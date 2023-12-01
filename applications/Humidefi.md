# Humidefi (The XGame platform)

- **Team Name:** Humidefi
- **Payment Address:** [5CfWkGnSnG89mGm3HjSUYHfJrNKmeyWgix5NKAMqePu4csgP] USDC/Polkadot
- **[Level](https://github.com/w3f/Grants-Program/tree/master#level_slider-levels):** 2

## Project Overview :page_facing_up:

If this application is in response to an RFP, please indicate this on the first line of this section.

If this is an application for a follow-up grant (the continuation of an earlier, successful W3F grant), please provide name and/or pull request of said grant on the first line of this section.

### Overview

#### Problem
Porting traditional game projects to Web3, which involves integrating blockchain and decentralized technologies, presents several challenges for game developers. 
1. Scalability Issues: Blockchain networks, especially those that are decentralized, may face scalability challenges, leading to slower transaction speeds and higher fees. This can impact the user experience in games that require a high level of interactivity and responsiveness.
2. User Onboarding and Complexity: Web3 games often require users to have a basic understanding of blockchain technology, wallets, and cryptocurrencies. Onboarding players who are new to these concepts can be challenging and may create a barrier to entry for mainstream audiences.
3. Transaction Costs: Transactions on blockchain networks typically involve fees. In a gaming environment, where microtransactions are common, these fees can become a significant concern, especially if they are relatively high or unpredictable.
4. Security Concerns: Blockchain transactions involve cryptographic keys, and the security of these keys is paramount. Developers must implement robust security measures to protect user assets and prevent unauthorized access or fraud.
5. Interoperability Challenges: Achieving interoperability between different blockchain networks and standards can be complex. Developers may face challenges when trying to integrate assets or data from one blockchain into another.

#### Solution
Humidefi is a Parachain in the Polkadot Ecosystem that has in-block Governance with Proof-Stake-Consensus mechanism, Smart Contracts and Decentralized Finace (DeFi) pallets and modules, e.g., stable coins, swaps, exchanges, loans, etc.  The main application of  Humidefi Parachain is XGame.  XGame provides a portal for game developers and virtual assets found in games and other multiverse activities to become real through the use of DeFi modules.
1. Scalability Issues: Parachains in the Polkadot network are designed to address scalability by allowing multiple blockchains (parachains) to run in parallel, rather than on a single chain. This parallel processing capability enhances the scalability of the entire Polkadot network. Humidefi as a Parachain is design to handle specific application geared toward Web3 Gaming with DeFi modules while running in parallel with the Polkadot network.
2.  User Onboarding and Complexity: XGame will provide the game developers and gamers user-friendly applications, e.g., NFT Marketplace, Dashboard Wallet, Exchange, etc., tailored fit to the needs of the define audience to be able to execute game Web3 porting with DeFi activities.  
3. Transaction Costs: Humidefi as a Parachain executes Layer 2 Solutions to mitigate transactions cost.  Layer 2 scaling solutions can offload  transactions from Polkadot to a Parachain. These solutions, such as sidechains or state channels, can significantly reduce transaction costs and increase throughput since all processing are done in the Layer 2 blockchain while Polkadot will only provide block validation and security.
4. Security Concerns: Polkadot employs a shared security model, where the security of the entire network is collectively provided by the relay chain. Instead of each parachain having to secure itself, they benefit from the security guarantees of the relay chain. This means that all parachains are secured by the same set of validators, promoting a higher level of security for the entire ecosystem.
5. Interoperability Challenges: Adopt standardized token standards for in-game assets and currencies. Following common standards such as ERC-20 or ERC-721 for Ethereum or standards specific to Polkadot parachains helps ensure that assets can easily move between different blockchains.  Furthermore, we can leverage Polkadot's Inter-Parachain Communication (XCMP) protocol to enable cross-chain messaging. This allows different parachains to communicate and share information, facilitating interoperability between games running on separate parachains.

### Project Details

#### Architecture

![Humidefi](https://drive.google.com/uc?id=1HZoU201KztQr-1L5yFV-bqtvGeOIX8Rb)

#### Technologies

1. [**Substrate**](https://substrate.io/) - Humidefi is a custom parachain using Substrate, change of behavior in Humidefi is done by modifying the code that specifies the rules and functionality unique to Substrate. It includes
    1. Runtime Modules: These are components of the blockchain that define the rules for transactions, state transitions, and other aspects of the blockchain's behavior.
    2. Smart Contracts: If the blockchain supports smart contracts, developers can include code for these contracts within the parachain code.
    3. Consensus Mechanism: The code also includes the rules for achieving consensus within the parachain, determining how blocks are produced and validated.
    4. Custom Features: Developers can implement custom features, governance mechanisms, or any other functionality they want the parachain to support.
2. [**Ink!**](https://use.ink/) - is a smart contract library specifically developed for Substrate. It provides a set of tools, abstractions, and utilities that make it easier for developers to write smart contracts on the Substrate framework.
    1. Rust Programming Language: ink! smart contracts are written in the Rust programming language, which is known for its performance, safety, and expressive syntax.
    2. Integration with Substrate: ink! is tightly integrated with the Substrate framework, allowing developers to leverage Substrate's modular architecture and features when building their smart contracts.
3. [**Polkadot.JS**](https://polkadot.js.org/docs/) - is a collection of JavaScript libraries and tools provided by Parity Technologies for interacting with the Polkadot network and Substrate-based blockchains. It is a suite of tools that includes various libraries and applications, enabling developers and users to interact with the Polkadot and Substrate ecosystems.
4. [**Node.JS**](https://nodejs.org/en/docs) - is an open-source, cross-platform JavaScript runtime environment that executes JavaScript code outside of a web browser. It is designed to build scalable and high-performance network applications. Node.js is built on the V8 JavaScript runtime engine, which is the same engine that powers the Google Chrome browser. It allows the team to use JavaScript for server-side scripting, enabling the development of server-side applications using a single programming language.
5. [**Angular**](https://angular.io/) - is a powerful open-source front-end web application framework maintained by Google. Angular is written in TypeScript, a superset of JavaScript that adds static typing to the language.  Key features and concepts of Angular include:
    1. Component-Based Architecture: Components encapsulate the application's logic, structure, and styling, promoting reusability and maintainability.
    2. Two-Way Data Binding: This feature allows automatic synchronization of data between the model and the view, eliminating the need for manual DOM manipulation.
    3. Dependency Injection: Angular uses a hierarchical dependency injection system, making it easy to manage and inject dependencies throughout an application.
    4. Directives: Angular introduces a powerful set of directives, including structural directives like ngIf and ngFor, which enable dynamic manipulation of the DOM.
    5. Services: Services in Angular are singletons that provide a way to encapsulate and share functionality across components. 
    6. Routing: Angular provides a powerful routing system for building single-page applications. 
    7. Observables and Reactive Programming: Angular leverages reactive programming and observables for handling asynchronous operations, such as HTTP requests.
6. [**MySQL**](https://www.mysql.com/) - is an open-source relational database management system (RDBMS) that is widely used for managing and organizing structured data. It is part of the LAMP stack (Linux, Apache, MySQL, PHP/Python/Perl) and is often used in conjunction with web applications to store and retrieve data.
7. [**Unity**](https://unity.com/) - is a powerful and widely used cross-platform game development engine and framework. It allows developers to create 2D, 3D, augmented reality (AR), and virtual reality (VR) applications for various platforms, including desktops, consoles, mobile devices, and the web. 

#### Components

1. [**Humidefi Parachain Node**](https://polkadot.js.org/apps/?rpc=wss%3A%2F%2Fhumidefi-dev.zeeve.net%2Fpara#/explorer)  - Humidefi is a parachain that connects to the Polkadot relay chain, which serves as the main chain in the network. Humidefi is customized and designed to serve gaming and metaverse activity purpose, e.g., XGame, with built-in decentralized finance modules.
    1. Consensus: Nominated Proof-of-Stake (NPoS), NPoS allows token holders, known as nominators, to nominate validators. Nominators essentially back validators by placing their stake behind them, increasing the validator's chance of being selected to produce blocks.
    2. Decetralized Finance (DeFi) Module: A DeFi module is a set of pallets within the Humidefi Parachain. This module would contain the logic, storage items, and dispatchable functions related to decentralized finance operations.
    3. Smart Contracts Module: Enabling pallet_contracts which provides support for smart contracts on Humidefi Parachain.  It allows developers to deploy, interact with, and manage smart contracts in Humidefi Parachain. This module is designed to work with the Ink! smart contract library.
    4. Governance: To add governance in Humidefi Parachain it will involve setting up the necessary modules and parameters to enable decentralized decision-making and on-chain governance mechanisms through the pallet_democracy module.
    5. Interoperability: Humidefi Parachain will implement the Cross-Chain Message Passing (XCMP) protocol. XCMP allows messages to be passed between parachains, enabling interoperability.
2. **Smart Contracts**  - ink! allows developers to write smart contracts in Rust, a systems programming language known for its performance, memory safety, and expressive syntax.   
    1. Substrate Integration: ink! is designed to seamlessly integrate with Substrate, a modular blockchain framework. Substrate allows developers to customize the blockchain runtime, and ink! provides the smart contract logic within this runtime.
    2. WebAssembly (Wasm) Execution: Smart contracts written using ink! are compiled to WebAssembly (Wasm), a binary instruction format that is designed to be executed at near-native speed in a safe and efficient manner. Wasm allows for cross-platform execution, making smart contracts portable across different blockchain environments.
3. **Rest API** - A RESTful API adheres to a set of principles that enable the creation of scalable and interoperable services. These principles include the use of standard HTTP methods (GET, POST, PUT, DELETE), stateless communication, resource-based URLs, and a uniform interface.
    1. [Fastify](https://fastify.dev/): Fastify is a web framework for building efficient and low-overhead web applications in Node.js. It is designed to be lightweight, highly performant, and focused on speed. Fastify is known for its minimal overhead, which makes it one of the fastest web frameworks available for Node.js.
    2. [Polkadot.JS](https://polkadot.js.org/docs/):  A suite of tools that includes various libraries and applications, enabling back-end developers and users to interact with the Humidefi Parachain.
4. **Web App** - All web apps in XGame and Humidefi will be built using Angular.
    1. [Homepage](https://www.xgame.live): The main page or entry point of XGame that is part of the Humidefi ecosystem. A user interface for all decentralized applications in XGame as well as all contents related to XGame, e.g., Blogs, News and Updates, Game Catalog, etc.
    2. [NFT Marketplace](https://nft.xgame.live): A web application designed to facilitate the buying, selling, and trading of digital assets represented as NFTs.  NFTs are unique cryptographic tokens that are often used to represent ownership of digital or physical items in XGame. 
    3. [Dashboard Wallet](https://dashboard.xgame.live): A user interface that allows individuals to interact with their Humidefi wallets and manage their blockchain-based assets and activities. The dashboard wallet enables the users to securely store, manage, and transact with their blockchain-based assets, including cryptocurrencies and non-fungible tokens (NFTs).
    4. [Exchange](https://exchange.xgame.live): A cryptocurrency exchange that operates within the Humidefi ecosystem.  XGame exchange leverages blockchain and decentralized finance (DeFi) principles to offer users greater control over their funds and a more trustless trading experience.
5. **Mobile App Wallet** - A mobile application that enables users to interact with and manage their cryptocurrency assets including NFT and decentralized applications (DApps) built on Humidefi.  The app serves also a the gateway for the gaming catalog of XGame.
6. **Games** - Web3 games built on Unity that leverages Humidefi Parachain features for various purposes, including asset ownership, decentralized finance (DeFi) mechanics, and play-to-earn models.

### Ecosystem Fit

1. **Attract Users to Polkadot Ecosystem** - A gaming platform like XGame can bring users to Polkadot ecosystem through Humidefi Parachain.  With in-game assets as non-fungible tokens (NFTs). This provides users with true ownership of digital assets, and these NFTs can potentially be used across different projects within the Polkadot ecosystem.
2. **Game Developers** - Simplifying entry into Web3 gaming and making it cost-effective through XGame involves a combination of user-friendly features, efficient onboarding processes, and strategic partnerships.  
    1. User-Friendly Onboarding: Create a seamless and user-friendly onboarding process. Minimize the technical barriers for users to get started with Web3 gaming on XGame. This includes easy account creation, clear instructions, and a straightforward way for users to acquire any necessary cryptocurrency or tokens.
    2. Wallet Integration: Build our own Mobile App Wallet. This can simplify the process of managing digital assets and interacting with the blockchain for users who may be new to Web3 gaming.
    3. Gas Fee Optimization: Implement strategies to optimize or mitigate gas fees associated with blockchain transactions. 
    4. Play-to-Earn Mechanics: Integrate play-to-earn mechanics that allow users to earn rewards or tokens by participating in the game. This incentive can attract users who are interested in earning value from their gaming activities.
    5. Cross-Platform Accessibility: Ensure that XGame is accessible across various platforms, including desktop and mobile devices. This widens the potential user base and accommodates users with different preferences and devices.
    6. Reduced Entry Costs: Explore ways to reduce the initial entry costs for users. This could involve providing starter packs, limited-time promotions, or discounted entry fees to encourage users to try out XGame without a significant upfront investment.
3. **DeFi for Game Developers and Gamers** - DeFi (Decentralized Finance) offers game developers a range of opportunities to innovate, monetize, and enhance the gaming experience in Polkadot Ecosystem.
    1. Tokenization of In-Game Assets: Use DeFi protocols to tokenize in-game assets as NFTs (Non-Fungible Tokens). This provides players with true ownership, enabling them to buy, sell, or trade these assets on XGame NFT Marketplace.
    2. Decentralized Exchanges (DEX): XGame Exchange enables seamless trading of in-game assets and tokens. This allows players to trade within the game or across different games, fostering a more dynamic and open economy.
    3. Play-to-Earn Models: Implement DeFi-based play-to-earn models where players can earn cryptocurrency or in-game tokens by participating in the game. This could involve completing quests, achieving milestones, or contributing to the overall game ecosystem.
    4. Liquidity Pools for In-Game Tokens: Create liquidity pools for in-game tokens on DeFi platforms. This ensures liquidity and stability for the in-game economy, allowing players to easily buy or sell tokens without facing significant price slippage.
    5. Incentive Mechanisms for Developers: DeFi can be used to create incentive structures for game developers, such as yield farming or staking, encouraging active participation in the ecosystem and rewarding continuous development efforts.
    6. Decentralized Funding for Game Development: Explore decentralized lending and borrowing platforms to fund specific aspects of game development. This can provide an alternative to traditional funding sources and involve the community in supporting the project.
4. [**Wemix**](https://www.wemix.com/wemix) - WEMIX3.0 is a high-performance EVM-compatible open source protocol powered by SPoA(Stake-based Proof of Authority) consensus algorithm which is secured by 40 decentralized authority nodes operated by highly-qualified global partners as well as on-chain community DAO(Decentralized Autonomous Organization). It is designed to be a robust and efficient platform-driven & service-oriented public blockchain home to innovative projects and applications built by community members and available to the world. 
    1. Blockchain: WEMIX3.0 is a forked Ethereum independent blockchain source code while Humidefi is a side chain than runs in parallel with Polkadot (Parachain).  Being a parachain in the Polkadot network offers many advantages compared to being an independent blockchain, for example; Shared Security, Interoperability, Scalability, Economic Efficiency, Cross-Chain Token Transfers, Upgradability and Ease of Integration.
    2. Applications: 
5. **XGame Strategy**

## Team :busts_in_silhouette:

### Team members

* Engr. Harold Glenn Minerva
* Noah Oliver Rigonan
* Oliver Enciso
* Caesar Ditan
* Ernesto Almario
* Joel Villena
* Michael Ian Kurt Descalso 
* Richlyn Vergara

### Contact

- **Contact Name:** Harold Glenn P Minerva
- **Contact Email:** hgminerva@liteclerk.com
- **Website:** https://www.liteclerk.com

### Legal Structure

- **Registered Address:** 
Liteclerk Corporation
211 V. Rama Avenue Corner B. Rodriguez St. 
Cebu City, Philippines, 6000
- **Registered Legal Entity:** 
Liteclerk Corporation
SEC No.: CS201811079

### Team's experience

* Engr. Harold Glenn Minerva
* Noah Oliver Rigonan
* Oliver Enciso
* Caesar Ditan
* Ernesto Almario
* Joel Villena
* Michael Ian Kurt Descalso 
* Richlyn Vergara

### Team Code Repos

#### Humidefi 
* Parachain: https://github.com/Blockspace-Corporation/humidefi-parachain-v2

#### XGame 
* XGame Homepage: https://github.com/oress-ph/oress-xgame-homepage-ui
* XGame NFT Marketplace: https://github.com/oress-ph/oress-xgame-marketplace-ui
* XGame Dashboard: https://github.com/oress-ph/oress-xgame-dashboard-ui
* Exchange UI: https://github.com/oress-ph/oress-xgame-exchange-ui
* Exchange API: https://github.com/oress-ph/oress-xgame-exchange-api
* Exchange Datasource (Binance): https://github.com/oress-ph/oress-xgame-exchange-web-socket
* Mobile Wallet:
* AstroChibbi Rest API:
* AstroChibbi Smart Contracts:

#### Team Github Profile
* Engr. Harold Glenn Minerva - https://github.com/hgminerva
* Noah Oliver Rigonan - https://github.com/oliverrigonan 
* Oliver Enciso - https://github.com/encisooliver
* Ernesto Almario - https://github.com/ernesr456
* Joel Villena - https://github.com/villenaj
* Michael Ian Kurt Descalso - https://github.com/kurtdescalso 
* Richlyn Vergara - https://github.com/richlynvergara 

### Team LinkedIn Profiles (if available)

* Engr. Harold Glenn Minerva - https://www.linkedin.com/in/harold-glenn-minerva-1789a254/
* Noah Oliver Rigonan - https://www.facebook.com/profile.php?id=100000558750786
* Oliver Enciso - https://www.linkedin.com/in/oliverenciso/ 
* Caesar Ditan - https://www.linkedin.com/in/caesarditan/ 
* Ernesto Almario - https://www.linkedin.com/in/ernesto-almario-4a9162191/
* Joel Villena - https://www.linkedin.com/in/villenaj43
* Michael Ian Kurt Descalso - https://www.linkedin.com/in/michael-ian-kurt-descalso-b55778259/ 
* Richlyn Vergara - https://www.linkedin.com/in/richlyn-c-vergara-169562199/ 

## Development Status :open_book:


### Proof of Concept



If you've already started implementing your project or it is part of a larger repository, please provide a link and a description of the code here. In any case, please provide some documentation on the research and other work you have conducted before applying. This could be:

- links to improvement proposals or [RFPs](https://github.com/w3f/Grants-Program/tree/master/docs/RFPs) (requests for proposal),
- academic publications relevant to the problem,
- links to your research diary, blog posts, articles, forum discussions or open GitHub issues,
- references to conversations you might have had related to this project with anyone from the Web3 Foundation,
- previous interface iterations, such as mock-ups and wireframes.

## Development Roadmap :nut_and_bolt:

This section should break the development roadmap down into milestones and deliverables. To assist you in defining it, we have created a document with examples for some grant categories [here](../docs/Support%20Docs/grant_guidelines_per_category.md). Since these will be part of the agreement, it helps to describe _the functionality we should expect in as much detail as possible_, plus how we can verify and test that functionality. Whenever milestones are delivered, we refer to this document to ensure that everything has been delivered as expected.

Below we provide an **example roadmap**. In the descriptions, it should be clear how your project is related to Substrate, Kusama or Polkadot. We _recommend_ that teams structure their roadmap as 1 milestone ≈ 1 month.

> :exclamation: If any of your deliverables is based on somebody else's work, make sure you work and publish _under the terms of the license_ of the respective project and that you **highlight this fact in your milestone documentation** and in the source code if applicable! **Projects that submit other people's work without proper attribution will be immediately terminated.**

### Overview

| No. | Milestone | Target Completion |
| -----: | ----------- | ------------- |
| **1** | Humidefi | 2022 |
| **2** | XGame | 2023 - 3rd Quarter |
| **3** | DEVNET | 2023 - 4th Quarter |
| **4** | TESTNET | 2024 - 1st Quarter |
| **5** | MAINNET | 2024 - 2nd Quarter |
| **6** | Game Developer Portal | 2024 - 4th Quarter |
| **7** | DeFi Modules | 2025 |
| **8** | PoS/DAO | 2026 |

- **Total Estimated Duration:** Duration of the whole project (e.g. 2 months)
- **Full-Time Equivalent (FTE):**  Average number of full-time employees working on the project throughout its duration (see [Wikipedia](https://en.wikipedia.org/wiki/Full-time_equivalent), e.g. 2 FTE)
- **Total Costs:** Requested amount in USD for the whole project (e.g. 12,000 USD). Note that the acceptance criteria and additional benefits vary depending on the [level](../README.md#level_slider-levels) of funding requested. This and the costs for each milestone need to be provided in USD; if the grant is paid out in Bitcoin, the amount will be calculated according to the exchange rate at the time of payment.

### Milestone 1 : Humidefi - The Parachain
- **Estimated duration:** 12 months
- **FTE:**  1,5
- **Costs:** 5,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| **1.1** | Rust | Learn Rust as a team.|
| **1.2** | Substrate | Clone Substrate Node Template and run a blockchain node.|
| **1.3** | Polkadot.Js | Communicate to the blockchain node use Polkadot.Js libraries.|
| **1.4** | Polkadot.Js | Communicate to the blockchain node use Polkadot.Js libraries.|

### Milestone 2 : XGame - The Web3 Gaming Platform
- **Estimated duration:** 1 month
- **FTE:**  1,5
- **Costs:** 8,000 USD

### Milestone 3: DEVNET - XGame and Humidefi Integration
- **Estimated duration:** 1 month
- **FTE:**  1,5
- **Costs:** 8,000 USD

### Milestone 4: TESTNET - In-game Economy, Web3 Wallet and NFT Marketplace
- **Estimated duration:** 1 month
- **FTE:**  1,5
- **Costs:** 8,000 USD

### Milestone 5: MAINNET - Mobile Wallet, Payment Portal and Community Engagement
- **Estimated duration:** 1 month
- **FTE:**  1,5
- **Costs:** 8,000 USD

### Milestone 6: Game Developer Porta - Portal for Smart Contracts and Tokens
- **Estimated duration:** 1 month
- **FTE:**  1,5
- **Costs:** 8,000 USD

### Milestone 7: DeFi - Exchange, Swaps, Loans, and other DeFi applications
- **Estimated duration:** 1 month
- **FTE:**  1,5
- **Costs:** 8,000 USD

### Milestone 8: PoS / DAO - Change to PoS consensus with governance
- **Estimated duration:** 1 month
- **FTE:**  1,5
- **Costs:** 8,000 USD




- **Estimated duration:** 1 month
- **FTE:**  1,5
- **Costs:** 8,000 USD

> :exclamation: **The default deliverables 0a-0d below are mandatory for all milestones**, and deliverable 0e at least for the last one. 

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| **0a.** | License | Apache 2.0 / GPLv3 / MIT / Unlicense |
| **0b.** | Documentation | We will provide both **inline documentation** of the code and a basic **tutorial** that explains how a user can (for example) spin up one of our Substrate nodes and send test transactions, which will show how the new functionality works. |
| **0c.** | Testing and Testing Guide | Core functions will be fully covered by comprehensive unit tests to ensure functionality and robustness. In the guide, we will describe how to run these tests. |
| **0d.** | Docker | We will provide a Dockerfile(s) that can be used to test all the functionality delivered with this milestone. |
| 0e. | Article | We will publish an **article**/workshop that explains [...] (what was done/achieved as part of the grant). (Content, language and medium should reflect your target audience described above.) |
| 1. | Substrate module: X | We will create a Substrate module that will... (Please list the functionality that will be implemented for the first milestone. You can refer to details provided in previous sections.) |
| 2. | Substrate module: Y | The Y Substrate module will... |
| 3. | Substrate module: Z | The Z Substrate module will... |
| 4. | Substrate chain | Modules X, Y & Z of our custom chain will interact in such a way... (Please describe the deliverable here as detailed as possible) |
| 5. | Library: ABC | We will deliver a JS library that will implement the functionality described under "ABC Library" |
| 6. | Smart contracts: ... | We will deliver a set of ink! smart contracts that will...


### Milestone 2 Example — Additional features

- **Estimated Duration:** 1 month
- **FTE:**  1,5
- **Costs:** 8,000 USD

...


## Future Plans

Please include here

- how you intend to use, enhance, promote and support your project in the short term, and
- the team's long-term plans and intentions in relation to it.

## Referral Program (optional) :moneybag: 

You can find more information about the program [here](../README.md#moneybag-referral-program).
- **Referrer:** Name of the Polkadot Ambassador or GitHub account of the Web3 Foundation grantee
- **Payment Address:** BTC, Ethereum (USDC/DAI) or Polkadot/Kusama (USDT) payment address. Please also specify the currency. (e.g. 0x8920... (DAI))

## Additional Information :heavy_plus_sign:

**How did you hear about the Grants Program?** Web3 Foundation Website / Medium / Twitter / Element / Announcement by another team / personal recommendation / etc.

Here you can also add any additional information that you think is relevant to this application but isn't part of it already, such as:

- Work you have already done.
- If there are any other teams who have already contributed (financially) to the project.
- Previous grants you may have applied for.
