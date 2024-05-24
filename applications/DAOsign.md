# EOS Network Foundation Grant Proposal

- **Project Name:** DAOsign
- **Team Name:** DAOsign, LLC
- **EOS Payment Address:** Ethereum Address - 0x793F7a7542c14088dbF58A19d2687FB9E7A79482; EOS Address - TBD
- **[Level](https://github.com/eosnetworkfoundation/grant-framework#grant-levels):** 2
- **Pomelo Grant(s):** N/A
- **Project is Open-Source:** Yes
- **Project was part of Token sale:** No
- **Repository where Project resides:** https://github.com/DAOsign

## Contact

- **Contact Name:** Eugene Fine
- **Contact Email:** eugene@daosign.org
- **Website:** https://daosign.org/


## Project Overview


### Overview

- **Name:** DAOsign is a Workflow Management platform built with a decentralized Smart Signature protocol
- **Brief Description:**

DAOsign offers a decentralized and customizable platform where collaboration, authorization, and workflow management are facilitated through cryptographic proofs stored on a blockchain

The Decentralized Smart Signature protocol serves as the cornerstone technology of DAOsign, encompassing a comprehensive system of cryptographic proofs, including identity, authority, signature, and agreement.

With Smart Signature, users gain access to a secure and customizable workflow management system. It also allows for control over team authorities and the ability to verify the signet’s identity.

- **Relationship to EOS Network / Antelope:** We offer to build DAOsign platform on the top of the EOS blockchain, allowing users to store their proofs on its chain.
- **Reason for Interest:** We believe that there is no reason for companies to rely on outdated technologies when signing agreements. Also, there is a significant lack of web3 workflow management platforms. Our goal is to address these issues and become the most secure and transparent platform on the blockchain.

### Project Details
DAOsign is already on the Testnet: https://testnet.daosign.org/connect. Currently, we support blockchains like Ethereum, Sui, Polkadot, and Oasis. We would be happy to add EOS to our list.

**DAOsign Interface**
- Landing page, where you can connect with your wallet
![image](https://github.com/TetianaRiabova/grant-framework/assets/122782612/aeed3840-7ffb-49c9-baad-0e02804d9300)

- User’s profile
![image](https://github.com/TetianaRiabova/grant-framework/assets/122782612/8ab09333-b0be-41e8-9dfc-4eaea5155189)

- Agreements
![image](https://github.com/TetianaRiabova/grant-framework/assets/122782612/ee7728ec-84e8-4281-9aae-c457ee57abf0)

- New Agreement creation
![image](https://github.com/TetianaRiabova/grant-framework/assets/122782612/4b47e590-d479-469e-8848-e9e48039ae8d)

- Configurations (Privacy, location, network)
![image](https://github.com/TetianaRiabova/grant-framework/assets/122782612/e28f2038-2e3d-4ccf-a060-46b76afeec96)

- Draft Page
![image](https://github.com/TetianaRiabova/grant-framework/assets/122782612/ad25547d-a540-448b-a30e-a13c34208609)

- Signed Document
![image](https://github.com/TetianaRiabova/grant-framework/assets/122782612/3e63a37a-ad58-4c2c-89f0-138c1637c393)

- Proof-of-Signature
![image](https://github.com/TetianaRiabova/grant-framework/assets/122782612/aa355a4b-5dca-41e1-b918-3456ecac11c2)

**Technical design**

Proofs are implemented in the EIP-712 standard and adjusted to ink! ecosystem. Proofs digned using user’s EVM private key. We are supporting this standard in Ink! smart contract to be able to verify the signature in ink! smart contract. Also, we are implementing an adjusted EIP-2771 standard to allow Agreement Signers gas-free delegation to publish proof on-chain. EIP-712 standard will be used for proofs, adaptation means that user data is converted to a binary bit; we use its hash (serialization vs deserialization) And EIP-2771 standard - to securely send the proof and receive it. So that EVM standards will be adapted to ink! ecosystem requirements. Example (interfaces) of the smart contracts can be found here https://github.com/DAOsign/daosign-smart-contracts (Solidity version).   

**Off-chain Relayer**

Relayer is an off-chain component that accepts transaction (with EIP-712 signature from Metamask) from user, signs it and sends to the network. This app will be developed using following technology stack:

- Typescript/NodeJS

- express.js

- polkadot.js

### Ecosystem Fit

We propose building a DAOsign tool on top of the EOS blockchain, which will allow users to store their proofs on its chain. We haven't found any similar project within the EOS Ecosystem and would love to be the first to build a tool with such features and functionality. We believe that our platform will enhance security, transparency, and trust within the EOS ecosystem, and improve its governance. Our platform extends beyond the scope of DAOs and can be utilized by any web3 organizations needing to manage agreements/policies and handle related workflows.

As for our competitive landscape, we have two types of competitors: electronic signature platforms, like DocuSign or EthSign, and workflow automation platforms, such as Chronicled or Everledger. 

DAOsign key differentiations: 

- Cryptographic proofs stored on the blockchain: DAOsign excels in this area, offering robust security and verifiability.

- Identity Verification: DAOsign provides reliable identity verification mechanisms.

- Customizable Workflows: Users can tailor workflows to their specific needs.

- Workflow Library: DAOsign offers a comprehensive library of predefined workflows.

- Workflow Builder: Users can create custom workflows easily.

- Workspace Configurations: DAOsign allows flexible workspace setups.

- Team Collaboration with revocable NFT authorities: Enhanced collaboration features.

- Multichain Wallet / IPFS support: Supports multiple chains and decentralized storage.

- Proposal Import (DAOs on Snapshot): Seamless integration with DAO governance.

- Governance Management/Automation: Efficient governance tools.

- DeFi Support: DAOsign caters to decentralized finance use cases.

- Signature Verifications: Robust signature validation.

- White-labeling: Custom branding options.

## Team

### Team members

- **Team Leader:** Eugene Fine - CEO & Founder
- Ramil Amerzyanov - CTO
- Mikhail Kondratenko - Technical Lead
- Yevhen Butkovskyy - Product Manager

### Legal Structure
- **Registered Legal Entity:** DAOsign, LLC
- **Registered Address:** 2468 Brian Dr. Northbrook, IL 60062

### Team Experience

Eugene Fine (CEO & Founder) - Over 20 years of building, scaling, and managing technology organizations. Recent experience includes a CTO role at Explorer Surgical Corp., which was recently acquired by GHX, and VP of Engineering at GHX. Eugene is a founder at consideritdone.tech, a Blockchain/WEB3 development studio.

Ramil Amerzyanov (CTO) - 15+ years building complex technical architecture and software solutions., focusing on Blockchain/WEB3 technologies over the past 7 years. Recent projects include the Fractional CTO role at Landslide Network and CTO role at consideritdone.tech.

Mikhail Kondratenko (Lead Technical Architect) - 6+ years developing Blockchain/WEB3 technical architecture and software solutions. Recent projects include Lead Technical Architect roles at Akiva Capital Holdings and Avalaunch.

Yevhen Butkovskyy (Product Manager) - 6+ years managing Blockchain/WEB3 products and software implementation projects, experienced Agile Scrum Master and Product Owner. Recent projects include the management of Landslide Network and Avalaunch implementations

### Team Org Repos

- https://github.com/DAOsign

- https://github.com/ConsiderItDone


### Team Member Repos

- [Eugene Fine](https://github.com/ConsiderItDone)

- [Ramil Amerzyanov](https://github.com/ramilexe)

- [Mikhail Kondratenko](https://github.com/Brioline)

- [Yevhen Butkovskyy](https://github.com/eugeneBskyy)

### Team LinkedIn Profiles (if available)

- [Eugene Fine](https://www.linkedin.com/in/eugenefine/)
- [Ramil Amerzyanov](https://www.linkedin.com/in/ramil-amerzyanov/)
- [Mikhail Kondratenko](https://www.linkedin.com/in/mykhail-kondratenko-29209a205/)
- [Yevhen Butkovskyy](https://www.linkedin.com/in/yevhenbutkovskyy/)

## Development Status

DAOsign Testnet is available here: https://testnet.daosign.org/

DAOsign Ethereum smart contracts: https://github.com/DAOsign/ethereum-smart-contracts

DAOsign Polkadot smart contracts: https://github.com/DAOsign/polkadot-smart-contracts

## Development Roadmap

This section should break the development roadmap down into milestones and deliverables. To assist you in defining it, we have created a document with examples for some grant categories [here](../docs/grant_guidelines_per_category.md). Since these will be part of the agreement, it helps to describe _the functionality we should expect in as much detail as possible_, plus how we can verify and test that functionality. Whenever milestones are delivered, we refer to this document to ensure that everything has been delivered as expected.

Below we provide an **example roadmap**. In the descriptions, it should be clear how your project is related to the EOS ecosystem. We _recommend_ that teams structure their roadmap as 1 milestone ≈ 1 month.

For each milestone,

- make sure to include a specification of your software. _Treat it as a contract_; the level of detail must be enough to later verify that the software meets the specification.
- include the amount of funding requested _per milestone_.
- include documentation (tutorials, API specifications, architecture diagrams, whatever is appropriate) in each milestone. This ensures that the code can be widely used by the community.
- provide a test suite, comprising unit and integration tests, along with a guide on how to set up and run them.
- commit to providing Dockerfiles for the delivery of your project.
- indicate milestone duration as well as number of full-time employees working on each milestone.
- **Deliverables 0a-0c are mandatory for all milestones**, and deliverable 0e at least for the last one. If you do not intend to deliver one of these, please state a reason in its specification (e.g. Milestone X is research oriented and as such there is no code to test).


### Milestone Summary

- **Total Estimated Duration:** 3,5 months
- **Full-Time Equivalent (FTE):** 4 FTE
- **Total Costs:** $20,680

### Milestone 1 — EOS Testnet version

- **Estimated duration:** 1,5 months
- **FTE:**  4
- **Costs:** $14,880.00

| ID | Deliverable | Specification |
| ----- | ----------- | ------------- |
| 0a. | License | Apache 2.0 |
| 0b. | Documentation | We will provide both inline documentation of the code and a basic tutorial that explains how a user can sign an agreement storing proofs on the EOS blockchain. |
| 0c. | Testing Guide | Core functions will be fully covered by unit tests to ensure functionality and robustness. In the guide, we will describe how to run these tests. |
| 0d. | Docker | We will provide a Dockerfile(s) that can be used to test all the functionality delivered with this milestone. |
| 1. | Store proof on EOS blockchain | Add EOS Network to DaoSign frontend and backend |  
| 2. | Store proof on EOS blockchain | Add EOS Network RPC Endpoint to Relayer |  
| 3. | Store proof on EOS blockchain | Manual testing |  
| 4. | Store proof on EOS blockchain | Documentation |  
| 5. | DAOsign configuration | EOS instance setup | 
| 6. | DAOsign configuration | EOS instance configuration | 



### Milestone 2  — EOS Mainnet version

- **Estimated Duration:** 2 month
- **FTE:**  4
- **Costs:** $5,800

| ID | Deliverable | Specification |
| ----- | ----------- | ------------- |
| 0a. | License | Apache 2.0 |
| 0b. | Documentation | We will provide both inline documentation of the code and a basic tutorial that explains how a user can sign an agreement storing proofs on the EOS blockchain. |
| 0c. | Testing Guide | Core functions will be fully covered by unit tests to ensure functionality and robustness. In the guide, we will describe how to run these tests. |
| 0d. | Docker | We will provide a Dockerfile(s) that can be used to test all the functionality delivered with this milestone. |
| 0e. | Article | We will publish an article that describes what was done as part of the grant. (Content, language and medium should reflect your target audience described above.) |
| 1. | DevOps | Production Environment setup |  
| 2. | DevOps | Github Actions |  
| 3. | DevOps | Mainnet Release |  
| 4. | Blockchain | Smart Contracts deployment | 



## Future Plans

Our main goal and plan is to support as many blockchain networks as possible. Initially, we aim to support the first 10 chains and then expand to the top 100. Additionally, as we continue developing our product, we are exploring new use cases for DAOsign such as RWA Tokenization, Grant Management Workflow, and Staking Operations. We are actively reaching out to various networks that may be interested in DAOsign. Building a strong community is also a priority for us, which is why we are actively sharing posts, articles, and guides. If the grant would be approved, we would be happy to connect with the EOS community and Ecosystem and share more about DAOsign and its functionality.


## Additional Information

**How did you hear about the Grants Program?** EOS Network Foundation Website

### DAOsign Materials:

- DaoSign Website: www.daosign.org
- DaoSign Product Overview: http://product-overview.daosign.support
- DaoSign RWA Tokenization Backoffice: http://rwa-backoffice.daosign.support
- DaoSign Product Demo: http://product-demo.daosign.support
- DaoSign Testnet: https://testnet.daosign.org
- DaoSign Early Adopter Program and LOI: https://docsend.com/view/xsjjdh42gun28cww

### DAOsign Social Media:

- DAOsign Twitter: https://twitter.com/dao_sign

- DAOsign LinkedIn: https://www.linkedin.com/company/daosign/

- DAOsign Telegram: https://t.me/DAOsign

- DAOsign Discord: https://discord.gg/AwnhGFbT8Z

- DAOsign Medium: https://medium.com/@daosign

### DAOsign Traction:

Early Adopters - TradeFi, GenesisBlock, Emet Research, Pairwyse, Nodle

Grants - SUI, Polkadot, Mintbase, Oasis, The Planq

Hackathon Winners - #AEZBoost Hackathon winners, AI X DeFi Cook-off Hackathon winners by Oraichain and DoraHacks
