# Technical Grant Proposal - Itheum's Privacy Preserving Computing Framework (R&D POC)

* **Project:** Itheum's Privacy Preserving Computing Framework (R&D POC)

## Project Overview  

Itheum is a decentralised data brokerage. It's a cross-chain "Data DEX" that allows users to trade personal data securely on-chain (works on EVM chains). Itheum also allows for the storage of highly secure sensitive data within "Data Vaults" and we have a feature called the "Trusted Computation Framework" that brings the compute-to-the-data via privacy-preserving tech (like Secure Multi-Party Computation, Homomorphic Encryption and Zero-Knowledge Proofs). Itheum's other core features (peer-to-peer data trade, data NFTs, data coalitions DAOs) are gaining some traction but we want to also explore our options in the privacy-preserving compute space.

Itheum also has a deep integration with a web2 platform toolkit that enables the building of "data collection and analytics apps" - anyone can use this toolkit to build user data collection tools with built in outcome-oriented analytics. This product is already in the market and powers products like OKPulse (https://okpulse.life) and Red Heart Challenge (https://itheum.com/redheartchallenge). The aim of this product is to democratise data collection and analytics technology and to increase the quality of high quality, outcome oriented personal data.

The data from these apps can then be "claimed" by the data creators in our Data DEX (https://datadex.itheum.com) and then traded using our decentralised tools. (watch a demo here - https://www.youtube.com/watch?v=63BE4plzDzw)

 **What benefits will this project bring to the Alaya or PlatON ecosystem:**
PlatON's Whitepaper shows the concept of a "Data Market" that forms a key component in their ["Layer 2" architecture](https://medium.com/platon-network/platon-2-0-white-paper-decentralized-privacy-preserving-ai-network-part-2-what-is-platon-2-0-14e24cf4bf48). Itheum will enable real-world programs like "OKPulse" and "Red Heart Challenge" and then uses the `Data DEX` for cross-chain data sharing. Itheum requires a privacy-preserving layer to handle the private data sharing and compute. The successful integration between Itheum and PlayON will demonstrate this working in unison. i.e. Itheum will be a highly valuable PlatON "Data Market" for real-world data sharing use-cases.


### Project Details

![Itheum Data DEX](https://raw.githubusercontent.com/Itheum/devgrants/rebrand/img/poc-privacy-preserving-tech.png)

As part of this R&D POC (Proof of Concept) we'd like to demonstrate the privacy-preserving layer of our platform. In Itheum; this option is handled by the `Trusted Computation Framework (TCF)` and enables sensitive data from the "data collection and analytics apps" to be exchanged with buyers without exposing the identity of both the buyer and seller. So a seller should be able to share a "sample of sensitive data" and the buyer should be able to share a "sample algorithm" with their "expected result quality" and the trusted computation layer should mediate the execution of the compute. It should provide back the data quality score and the guarantee the buyer is using the data as per algorithm definition (i.e. the terms of the use are as per agreed on). This enables for the trade to happen via privacy preserving principles and without any intermediaries.

## How it works end-to-end:
The below is the end-result and ideal design. But for the POC, we may just setup a `sandbox that can replicate this` so we can test the PlatON integration. We can then move to formalise this later as part of another engagement.

**Product Overview:**
- We source and work with a "Research Partner" (essentially someone who can write the sample algorithms to run on the personal data provides by Itheum into PlatON)
- We work with the "Research Partner" to highlight the `type on input data that will be available` and then formulate the `type of algorithm` that will need to run on it to get desired results. The expected `data quality threshold and algorithm output` will also be agreed upon.
- We work together to identify a large POC user-base (i.e. Data Creators) that will provide their data.
- Itheum will launch a new 'Data Collection and Analytics' app build upon the existing `Red Heart Challenge` app/program foundation (there will be public onboarding link for this app. e.g. https://itheum.com/redheartchallenge)
- Our POC users (Data Creators) will be invited to participate in the `Red Heart Challenge` program.
- Our POC users (Data Creators) will use the `Itheum Data DEX` to link their web3 accounts to the core `Red Heart Challenge` program.
- The `Itheum Data DEX` will ingest all the personal data and make it available for web3 trade.

**Technical Overview:**

Itheum's `Trusted Computation Framework (TCF)` is a "virtual pools of Data Coalition (DC) DAOs". DC DOAs will integrate into the pool if all "Members" in the DOA agree to it. A Data Coalition (DC) is a DAO that can bulk sell data. A user can join a DC and allow it to sell their data. A user can also have a `Personal Data Vault` that locks in their demographics/sensitive personal data. The DC can have "delegated ownership" of Data Vault as well, in the event the "data requester" wants to identify the source of the data for any form of targeting (i.e. to notify original user that an anomaly is found in their data - we can show an alert to the original user in the Data DEX that an anomaly was detected in their data by "agents" within the Trusted Computation Framework)

1) Standup a new Data Coalition DAO that can collect data from the `Red Heart Challenge` program (e.g. `Privacy Preserving Cardiovascular Research` Data Coalition)
2) The DC DAO joins the `Trusted Computation Framework (TCF)`
3) The `Trusted Computation Framework (TCF)` integrates with the `PlatON Layer 1 and 2 - Consensus Network & Privacy Preserving Computation Network`
4) Once the "link" between PlatON and Itheum is completed; data under the management of the DC DAO is "shared" with the `data nodes within PlatON's blockchain`. How this works exactly is yet to be designed. i.e. how do we move Itheum personal data into PlatON without duplicating, leaking privacy or impacting the data veracity (in Itheum, the veracity is achieved via `Personal Data Proofs`). Will it be via a smart contract bridge or some other API? based on the technical design of PlatON, `Itheum will become a "Data Market" in PlatON's Layer 2 architecture.`
5) Once the data is shared with PlatON, it will be kept "invisible" but yet be available for use via a scheme like secure multipart computing or federated learning. Algorithms by the "Research Partner Agents" then run on the data but the results will also be kept secure. If an anomaly in the data is detected, it should be able to submit a proof that can be matched on Itheum's platform to find the original data creator/submitted and raise an alert within the Data DEX.


**The "end-vision" being:**
As a Data Creator - I'm going to keep my personal demographic data in my Data Vault and my longitudinal health data is always connected to a DC DAO. The DC DOA will share the longitudinal health data plus any "avatar based demographics" (i.e. not actual PII but representative PII, for e.g. we wont send the actual DOB but an `age group`) to PlatON where there are "agents" who can detect anomalies in the datasets by executing algorithms against the data. If an anomaly is detected, the PlatON smart contracts should be able to interface with the Itheum contracts via proofs to notify the original data creator of the data anomaly. All these steps need to happen without ever leaking the true identity of the data creator.


### Project Advantages
The initial version of Ocean Protocol was doing something similar (i.e. to enable privacy preserving computation) but we are not sure if they progressed with it. This may be because they were trying to build this framework themselves. Itheum intends to partner with a privacy preserving SME partner so we don't "reinvent the wheel" and can focus on building the entire personal data sharing ecosystem protocol that coordinates the end-to-end lifecycle.

### Project Code Repos
https://github.com/Itheum

## Team
* Itheum

### Team members

- https://www.linkedin.com/in/markpaulweb/
- https://www.linkedin.com/in/mkhanal/
- https://www.linkedin.com/in/dineish/

### Contact
* Mark Paul
* **contact details:** Twitter (https://twitter.com/itheum), Discord (https://discord.gg/y77P9gKF27), Telegram (https://t.me/joinchat/e000AVkV5RU4Zjc1)
* **Website:** https://itheum.com

### Team's experience
As a team we each have over 20 years experience in the software engineering, technology, data and security industry and have worked for the some of the largest global corporates (spanning Government, Banking, Consulting, Media etc). We are now moving into the blockchain tech space to solve the "public/social goods" issue around data governance, data sharing and personal data sovereignty.

## Development Roadmap
We are aiming to keep it simple and propose a 2 milestone development that can demonstrate the Itheum and PlatON integration. This is more pragmatic we feel given the complexity of what we are trying to do. This also increases the possibility of success.

### Overview
* **Total Estimated Duration: 5 months** 
* **Full-Time Equivalent (FTE): 3**
* **Total Costs::** $90k


### Milestone 1 —— Itheum's Trusted Computation Framework integration with PlatON - Let's call it the "Itheum/PlatON Link"
* **Estimated duration:** 2 months
* **FTE:**  2
* **Costs:** 45,000 USD


| Number | Deliverable | Specification |
| ------------- | ------------- | ------------- |
| 0a. | License | Open Source License as appropriate |
| 0b. | Documentation | We will provide code description documents and basic tutorials, which will explain how to use our products. |
| 0c. | Testing Guide	 | In order to ensure the integrity of the function and the robustness of the system, we will provide a test coverage of the code and explain how to run these test cases.| 
| 1. | Module 1: 1 | Work on efficient design to link our Trusted Computation Framework with PlatON Layer 1 and 2. Output will be an open source architecture document |
| 2. | Module 2: 2 | Work with PlatON team and finalise correct integration pattern (smart contracts, APIs, bridges, events, oracles etc) |
| 3. | Module 3: 3 | Build integration in a testnet sandbox (on Itheum's side and on PlatON's side) |
| 4. | Module 4: 4 | Setup a 'health-check' in Itheum's Data Dex where a user can ping the PlatON in real-time to make sure the integration is healthy and ready to accept new "jobs". |



### Milestone 2 —— Standup "Data Coalition + Red heart Challenge" sandbox
* **Estimated duration:** 3 months
* **FTE:**  3
* **Costs:** 55,000 USD


| Number | Deliverable | Specification |
| ------------- | ------------- | ------------- |
| 0a. | License | Open Source License as appropriate |
| 0b. | Documentation | We will provide code description documents and basic tutorials, which will explain how to use our products. |
| 0c. | Testing Guide	 | In order to ensure the integrity of the function and the robustness of the system, we will provide a test coverage of the code and explain how to run these test cases.| 
| 1. | Module 2: 1 | Setup new dedicated "Red heart Challenge" program that can be used as the "front-end" for data collection |
| 2. | Module 2: 2 | Setup a new dedicated Data Coalition (e.g. name will be `Privacy Preserving Cardiovascular Research` Data Coalition) |
| 3. | Module 2: 3 | The new Data Coalition is linked to the Itheum "Trusted Computation Framework" |
| 4. | Module 2: 4 | User's who join this program, can log into the Itheum Data DEX and link their data to a new Data Coalition |
| 5. | Module 2: 5 | The "trusted computation framework" can use the integration built in Milestone 1 to push data to PlatON's network for privacy preserving algorithm execution. For this POC, the job will need to run on-demand and send a "snapshot of bulk data" (in future we can auto-stream data over the Itheum/PlatON Link) |


### Next Steps:
If the above Milestones are successful; we can move to a more formal agreement between Itheum and PlatON where we can start working on completing the user experience (i.e. securely sharing the results of the algorithm execution and/or anomaly detection back to the original user in Itheum)

...

## Future Plans
- Itheum will become the core protocol to bring personal data into smart contracts. This will enable many more real-world examples to move on-chain. As such, privacy preserving tech is very important to us and we aim to grow stronger in this area with some strategic partners.

- We are also doing a lot of work with Filecoin who have an interesting idea that involves having "distributer compute near storage" - effectively, we can use FileCoin's decentralised storage for our data exchange medium and potentially co-locate decentralised sensitive, compute workloads into trusted hardware that is located neat the storage. We are exploring this design as part of our work with Filecoin and Hedera hashgraph and can potentially look at PlatON as a core component in our work.

- Once we deploy our solution as part of this Grant; we will support with it the same SLAs as all our other open source blockchain software. 

## Additional Information

We have very good progress and have many core features working in a MVP state in many EVM testnets, due to this progress we have been successful in many hackathons (polygon/elrod/moralis, harmony, hedera/filecoin etc). So we have a strong foundation to now start designing and building out a `Trusted Computation Framework (TCF)` powered by PlatON.

