# Humidefi (The XGame platform)

- **Team Name:** Humidefi
- **Payment Address:** [5CfWkGnSnG89mGm3HjSUYHfJrNKmeyWgix5NKAMqePu4csgP] USDC/Polkadot
- **[Level](https://github.com/w3f/Grants-Program/tree/master#level_slider-levels):** 2

## Project Overview :page_facing_up:

If this application is in response to an RFP, please indicate this on the first line of this section.

If this is an application for a follow-up grant (the continuation of an earlier, successful W3F grant), please provide name and/or pull request of said grant on the first line of this section.

### Overview

Humidefi is a blockchain platform that supports Smart Contracts and Decentralized Financial (DeFi) activities, e.g., stable coins, swaps, exchanges, loans, etc.

The main application on the Humidefi blockchain platform is XGame.  XGame provides a portal for virtual assets found in games and other multiverse activities to become real.  

On the first year of its operation, the Humidefi XGame node will integrate with Kusama then the succeding years would hopefully be Polkadot.  As more games being developed and deployed in XGame and more active users, our Decentralize Financial (DeFi) modules will eventually be deployed to help the users make the transfer from virtual to real.

### Project Details

#### Architecture

![Humidefi](https://drive.google.com/uc?id=1HZoU201KztQr-1L5yFV-bqtvGeOIX8Rb)

#### Technologies

1. Substrate
Humidefi is a custom parachain using Substrate, change of behavior in Humidefi is done by modifying the code that specifies the rules and functionality unique to the blockchain. It includes:
1.1. Runtime Modules: These are components of the blockchain that define the rules for transactions, state transitions, and other aspects of the blockchain's behavior.
1.1. Smart Contracts: If the blockchain supports smart contracts, developers can include code for these contracts within the parachain code.
1.1. Consensus Mechanism: The code also includes the rules for achieving consensus within the parachain, determining how blocks are produced and validated.
1.1. Custom Features: Developers can implement custom features, governance mechanisms, or any other functionality they want the parachain to support.

2. Ink!


3. Polkadot.JS
4. Node.JS
5. Angular
6. MySQL
7. Unity

#### Components

1. **Humidefi Parachain Node**  
2. **Smart Contracts**  
3. **Rest API (Dapps)**
4. **Polkadot.JS**
5. **Web Apps**
6. **Mobile Wallet**
7. **Games**

### Ecosystem Fit

Help us locate your project in the Polkadot/Substrate/Kusama landscape and what problems it tries to solve by answering each of these questions:

- Where and how does your project fit into the ecosystem?
- Who is your target audience (parachain/dapp/wallet/UI developers, designers, your own user base, some dapp's userbase, yourself)?
- What need(s) does your project meet?
- Are there any other projects similar to yours in the Substrate / Polkadot / Kusama ecosystem?
  - If so, how is your project different?
  - If not, are there similar projects in related ecosystems?

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
- Parachain: https://github.com/Blockspace-Corporation/humidefi-parachain-v2

#### XGame 
- XGame Homepage: https://github.com/oress-ph/oress-xgame-homepage-ui
- XGame NFT Marketplace: https://github.com/oress-ph/oress-xgame-marketplace-ui
- XGame Dashboard: https://github.com/oress-ph/oress-xgame-dashboard-ui

- Exchange UI: https://github.com/oress-ph/oress-xgame-exchange-ui
- Exchange API: https://github.com/oress-ph/oress-xgame-exchange-api
- Exchange Datasource (Binance): https://github.com/oress-ph/oress-xgame-exchange-web-socket

- Mobile Wallet:
- AstroChibbi Rest API:
- AstroChibbi Smart Contracts:

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

- **Total Estimated Duration:** Duration of the whole project (e.g. 2 months)
- **Full-Time Equivalent (FTE):**  Average number of full-time employees working on the project throughout its duration (see [Wikipedia](https://en.wikipedia.org/wiki/Full-time_equivalent), e.g. 2 FTE)
- **Total Costs:** Requested amount in USD for the whole project (e.g. 12,000 USD). Note that the acceptance criteria and additional benefits vary depending on the [level](../README.md#level_slider-levels) of funding requested. This and the costs for each milestone need to be provided in USD; if the grant is paid out in Bitcoin, the amount will be calculated according to the exchange rate at the time of payment.

### Milestone 1 Example — Basic functionality

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
