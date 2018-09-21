# Project name

WEEVE

# Project summary

Data is the new goal. But to harvest the value of data one needs to solve a fundamental problem: How to attest data? By attestation we mean a method that allows any third party to verify the truthfulness of the data. Otherwise fake data can be brought into systems, poisoning any AI engines or data marketplaces. Weeve solves the problem by providing method to implement trusted data oracles, using novel cryptographic proof techniques (“testimony”) to certify the data harvesting process and leveraging trusted execution environments/enclaves to shield sensitive parts of the software running on a device. In addition, weeve builds a platform to curate 2-sided data marketplaces, bringing supply and demand of IoT data together. The platform uses AI to define a nash equilibrium between suppliers and demanders and empowers IoT device to participate in a fair exchange fully autonomously while using cryptocoins to complete the trade. Weeve’s token model aims to increase the trust in a network of data suppliers, demanders and marketplace owners leveraging principles of staking to punish bad behavior (eg. fake data provisioning, curation of black market industries, plagiarism) and to reward good behavior (eg. verifying device membership standards, honesty of marketplace owners).

# Typical use case

Data Trading in Electric Vehicle Data Marketplace
Use Case:
An electric vehicle (EV) aims to charge energy from a station. The EV demands energy. Both player are equipped with an IoT device (eg microcontroller) running the weeveOS. Part of the weeveOS is a secure communication protocol (MQTTS) to transport data and a blockchain wallet (to provide a cryptographic identity and approve payments). Once the car connects to the station, the two players agree on the amount of energy. The IoT sensor at the gas station measures the energy transferred through the charging cable. A testimony (i.e. the cryptographic attestation) is computed and added to the check (encoded in a smart contract). The car can verify the check, before issuing a blockchain-based payment. The computation of the payment is testified as well and sent as an payment acknowledgment to the gas station. The testimony makes sure that no dispute arises, as each player can prove it complied with the fair exchange protocol and behaved correctly.

Tech:
Weeve OS, Weeve MQTTS, Weeve Testimony, Weeve Network, Blockchain
Partner:
Car manufacturer (or technology provider with access to car), energy provider (or charging station provider), any blockchain that suits scalability and fee model

# Stakeholders

|Name|More details|
|----|----|
|Device Owner|Register device on the network|
|Registry Owner|Create, Accept/Reject registry on network|
|Registry Participants|Upvote/Downvote devices based on pre defined parameters|
|Marketplace Creator|Create Marketplace on the network|
|Marketplace Participants|Trade data in the Marketplace|
|Validators|Accept registry listing|
|Externally Elected|Settle Disputes when arise in transactions|
|Delegated Council|Expert Pool of voters vote for the reputation of data streams|

# Token journey

||condition|stakeholder|action|token/inventive|objective|
|----|----|----|----|----|----|
|Step 0a|Token Acquisition(Through Token Sale or Exchange)|Device Owner|Stake|WEEV|Register device on the network|
|Step 0b|Token Acquisition(Through Token Sale or Exchange)|Registry Owner|Stake|WEEV|Create registry on network|
|Step 0c|Token Acquisition(Through Token Sale or Exchange)|Marketplace Creator|Stake|WEEV|Create Marketplace on network|
|Step 1|Registry Validation|Validators|Vote/Governance|WEEV|WEEV network validators accept registry listing|
|Step 2|Device Validation|Registry Owner|Accept|WEEV|Accept or Reject Device in Registry|
|Step 3|Grading|Registry Participants|Vote|WEEV|Registry Participants upvote or downvote devices based on predefined parameters|
|Step 4|Trading|Marketplace Participants|Trade|Agnostic|Trade data in the Marketplace|
|Step 5|Arbiter|Externally Elected|Dispute Resolution|WEEV|Settle Disputes when arise in transactions|
|Step 6|Experts|Delegated Council|Ranking|WEEV|Expert Pool of voters vote for the reputation of data streams|

# Token details

|Name|Symbol|More details|
|----|----|----|
|WEEV ERC-20 Token|WEEV|Tokens launched through a private sale, public sale and eventually listed on exchanges.|

# Current considerations:

* Incentivizing early participants to come to the network.
* Detect rogue participants early and prevent spamming of the network.
* Select a pricing mechanism for staking tokens on the TCR - Using pre defined parameters like device value, transaction type, transaction velocity to define an algorithm to decide the amount of stakes needed to enter a device.
* Network Incentivization - Launch a token sale for WEEV tokens with a limited pool of tokens, allow the remaining tokens supply and price to be determined through a bonding curve.
* Blockchain Macro Economic factors - Find out how sharding, plasma, state channels etc. would affective the network launch.