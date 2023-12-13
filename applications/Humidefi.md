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

![Humidefi Team](https://drive.google.com/uc?id=1Mt8QcdfRsF6o0T5tpmGYBEaSJO9OW_CI)

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

* Harold Glenn Minerva - An engineer by education with masters in business administration and a software architect by profession.  Over twenty (20) years of software engineering and development experience at which he founded three (3) software development companies wherein two (2) were already sold and one of which to a foreign investor.  He has solid expertise on C#  and Dot Net framework, PHP and Laravel framework, Javascript and Angular framework, Phython for machine learning and data science; and Rust for Web3 and Substrate platforms.  As a former CTO with a solid background in ITIL and process engineering, he can handle Cloud Infrastructures, e.g., AWS, Azure and Google Cloud and physical IT management using ISO 9001/27000 procedures .  The only consultant in the southern part of the Philippines for SYSPRO ERP.
* Noah Oliver Rigonan - A highly skilled and versatile software developer with a comprehensive set of expertise. His proficiency in Web3 technologies is evident through his adeptness in Substrate/Polkadot, Smart Contracts (Ink, Solidity), and NFT development. In the realm of programming languages, He excels in Rust/Substrate & Smart Contract, C#/ASP.NET, and demonstrates mastery in JavaScript, Typescript, Angular, and NodeJS for dynamic and interactive web applications. His capabilities extend into the realm of machine learning with expertise in Python, utilizing frameworks such as TensorFlow and PyTorch, as well as leveraging Python libraries like Pandas. Noah is equally adept in PHP/Laravel for web development and Java/J2EE Spring Framework for robust backend solutions. His cloud infrastructure proficiency covers GitHub integration, AWS services (EC2, RDS, ECR, etc.), Google Cloud technologies (Firebase, Google API, etc.), and Docker on Ubuntu-Linux for efficient containerization. Additionally, he has a strong background in AI, machine learning, and data science, utilizing HuggingFace Models and Transformers to enhance natural language processing capabilities. His database expertise includes SQL (MSSQL, MySQL & Oracle SQL), showcasing a well-rounded skill set that positions him as a valuable asset in the dynamic field of software development.
* Oliver Enciso - 
* Caesar Ditan - Over 40 years of top-level management, business development, sales, and marketing experience in IT (information technology), the academic, broadcast, advertising, and entertainment industries in various domestic, regional, and global markets; award-winning songwriter and record producer Mango Jam: Best of New Cebu Music Volume One, 1992; Master of Management post-graduate degree from the University of the Philippines.
* Ernesto Almario - A multifaceted professional with expertise across various domains in software engineering. As a Smart Contract Engineer, his proficiency extends to Front-end and Back-end development, showcasing his adeptness in technologies like TypeScript, Angular, Laravel, and Vue.js. His skill set includes Test-Driven Development, Git version control, and Manual Testing, ensuring robust and efficient software solutions. Ernesto's proficiency with Front-end engineer, Back-end engineer enables him to craft responsive web applications with meticulous attention to detail. With a keen eye for design using Figma and experience in Web Testing, he excels in creating user-centric, visually appealing, and functionally seamless applications. Ernesto's dedication to innovation and his comprehensive skill set make him a valuable asset in the realm of software engineering.
* Joel Villena - An experienced software engineer with a wide range of skills. He specializes in the roles of software engineer, smart contract engineer, and back-end engineer with a focus on REST API development. He has an impressive record in software engineering, has proven to be competent about blockchain technology by developing and running smart contracts. As an experienced back-end engineer, he has created and managed RESTful APIs with success, guaranteeing smooth communication between various aspects of complex structures. He combines technical knowledge with a commitment to providing excellent solutions, and offers a lot of expertise to the area. He places an emphasis on innovation and keeps up with the latest developments in the sector.
* Michael Ian Kurt Descalso - A versatile software engineer able to cover a wide range of roles, including but not limited to back-end APIs, web interfaces, and mobile applications. He has near 4 years of both freelancing and professional development experience combined under his wing. Michael has an interest in Linux systems and uses one on the daily. He has a particular preference for open-source and privacy respecting software, and keeps the philosophy in mind when building systems.
* Richlyn Vergara - With a background in education and a successful licensure examination under her belt, I transitioned into a dynamic role as an Executive Assistant, specializing in project management. Over the course of two years, she honed her skills by spearheading Product Implementation for Payroll Systems, showcasing her proficiency in managing complex tasks and ensuring seamless project execution.  Currently, she pivoted her career to the cutting-edge realm of Quality Assurance for Web3 projects. In this role, she leverage her expertise to uphold the highest standards of quality in the ever-evolving landscape of Web3 technologies. My journey reflects a commitment to continuous growth and a versatile skill set that spans education, project management, and quality assurance in the tech industry.
* Arneil Paul Polican - Skilled software developer with a proven track record spanning 3 years, specializing in VBA for SME client customization. Possesses 2+ years of expertise in both .NET Core and .NET Framework, along with 2+ years in Angular. Proficient in MSSQL with 5+ years of experience and a demonstrated ability to lead teams for over 2 years.

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

(To do)

### Proof of Concept

(To do)

## Development Roadmap :nut_and_bolt:

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

### Milestone 1 : Humidefi - The Parachain (Research and Development / Hackathons)
- **Estimated duration:** 12 months
- **FTE:**  1
- **Costs:** 5,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| **1.01** | Rust | Learn Rust as a team. |
| **1.02** | Substrate | Clone Substrate Node Template and run a blockchain node. |
| **1.03** | Polkadot.Js | Communicate to the blockchain node use Polkadot.Js libraries. |
| **1.04** | Humidefi App | Create a simple Angular Web App.  The initial objective is to connect a wallet and display the tokens and other assets. |
| **1.05** | Smart Contract Support | Add smart contracts in the Substrate node template. |
| **1.06** | DeFi Modules | Add a pallet_dex to the Substrate Node template. |
| **1.07** | Humidefi App with DeFi | Modify the existing Angular Web App to include swaps other DeFi functionalities in the pallet_dex. |
| **1.08** | ERC20 Smart Contract | Create and deploy an Ink! ERC20 Smart Contract. |
| **1.09** | Cumulus | Converting the standalone blockchain to a Parachain. |
| **1.10** | Relay Chain | Setting up a local Relay Chain that is needed by the Parachain. |
| **1.11** | Parachain | Connecting the local Parachain to the local Relay Chain. |
| **1.12** | Parachain Smart Contract | Add smart contracts to the Parachain. |

### Milestone 2 : XGame - The Web3 Gaming Platform
- **Estimated duration:** 3 months
- **FTE:**  9
- **Costs:** 30,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| **2.01** | XGame Requirements | XGame platform requirements and specifications analysis. |
| **2.02** | Game Catalog | XGame game catalog overview and documentation. Identification of games that can be ported to Web3. |
| **2.03** | Homepage | XGame Hompage using Angular. |
| **2.04** | Game Catalog | XGame Game Catalog Page. |
| **2.05** | Blogs | XGame Blog Page.  The content of the blog will be used to train the NLP chatbot. |
| **2.06** | Admin Page | XGame Admin Page for blogs, translation and other internal web data. |
| **2.07** | Homepage API | Rest API and corresponding database for the Homepage. |
| **2.08** | Middle Tier API | Rest API for Parachain connectivity. |
| **2.09** | Social Media Outlet | Create a social media outlet to start community engagement and to update the community on the status of XGame. |
| **2.10** | Machine Learning | Develop a machine learning model for XGame support using the blogs and other information posted in the Homepage. 
| **2.11** | Multi-language | XGame Homepage multi-language support and translation. |
| **2.12** | NFT Marketplace | XGame NFT Marketplace web app user interface using Angular. |
| **2.13** | Dashboard | XGame Dashboard web app user interface using Angular. |
| **2.14** | Exchange | XGame Exchange web app user interface using Angular. |
| **2.15** | Web Assets | Web Assets, e.g., posters, game logos and ads for XGame. |
| **2.16** | Homepage V2.0 | Redesign the XGame Homepage and other pages to include the Web Assets. Make the entire site consistent in terms of design and containers. |

### Milestone 3: DEVNET - XGame and Humidefi Integration
- **Estimated duration:** 3 months
- **FTE:**  9
- **Costs:** 30,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| **3.01** | Parachain | Humidefi Parachain WASM file and headers for deployment. |
| **3.02** | Humidefi-Genesis Node | Adding new node to the Humidefi Parachain. |
| **3.03** | Humidefi-Genesis Chainspec | Humidefi-Genesis DEVNET chainspec preparation. |
| **3.04** | DEVNET Deployment | DEVNET Deployment and Testing (c/o Infrastructure Provider). |
| **3.05** | Wallet Integration | Polkadot Wallet Integration. |
| **3.06** | NFT Marketplace DApp | Conversion of NFT Marketplace App to be able to connect to the Polkadot Wallet. |
| **3.07** | Dashboard DApp | Conversion of Dashboard App to be able to connect to the Polkadot Wallet. |
| **3.08** | ERC 721 | Creating of NFT contract using Ink! and deployment them to DEVNET. |

### Milestone 4: TESTNET - In-game Economy, Web3 Wallet and NFT Marketplace
- **Estimated duration:** 1 month
- **FTE:**  9
- **Costs:** 30,000 USD

| Number | Deliverable | Specification |
| -----: | ----------- | ------------- |
| **4.01** | Homepage Redesign | XGame Homepage redesign. |
| **4.02** | Humidefi-Genesis Chainspec | Humidefi-Genesis TESTNET chainspec preparation. |

### Milestone 5: MAINNET - Mobile Wallet, Payment Portal and Community Engagement
- **Estimated duration:** 6 Months
- **FTE:**  1,5
- **Costs:** 100,000 USD

TBD

### Milestone 6: Game Developer Porta - Portal for Smart Contracts and Tokens
- **Estimated duration:** 6 Months
- **FTE:**  9
- **Costs:** 100,000 USD

TBD

### Milestone 7: DeFi - Exchange, Swaps, Loans, and other DeFi applications
- **Estimated duration:** 12 Months
- **FTE:**  9
- **Costs:** 100,000 USD

TBD

### Milestone 8: PoS / DAO - Change to PoS consensus with governance
- **Estimated duration:** 12 Months
- **FTE:**  9
- **Costs:** 100,000 USD

TBD

## Future Plans

Based on the timeline and objective of the project, that it will be the go-to Web3 platform for game developers and gamers, our future plan is to give the platform autonomy and scalability for its intended users.

### Robust DeFi Modules

(To do)

### Decentralized Autonomous Organization

(To do)

