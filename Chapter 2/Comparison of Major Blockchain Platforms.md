# Comparison of Major Blockchain Platforms

Platform|Consensus Mechanism|Scalability|Programming Language|Use Cases
:---|:---|:---|:---|:---
Ethereum|PoW (Transitioning to PoS)|Working on Ethereum 2.0 for improved scalability|Solidity|General-purpose blockchain, decentralized applications
Quorum (ConsenSys)|Raft or Istanbul BFT|Focus on privacy and performance|Solidity|Enterprise solutions, finance
Hyperledger Fabric|Pluggable, supports various mechanisms|Modular architecture for scalability|Go, Java, Node.js|Supply chain, finance, enterprise solutions
Corda|Notary-based consensus|Designed for privacy and scalability|Kotlin, Java|Financial services, legal, supply chain
IBM Blockchain|Supports multiple mechanisms|Modular for different business needs|Go, Java|Supply chain, finance,healthcare
Bitcoin|PoW|Limited scalability, slower transaction processing|Bitcoin Script|Peer-to-peer digital currency
Hyperledger Sawtooth|PoET (Pluggable)|Modular design for flexibility|Python, Go|Supply chain, finance
Stellar|Federated Byzantine Agreement (FBA)|High throughput and fast settlement|Stellar (custom language)|Cross-border payments, remittances
Ripple|Ripple Protocol Consensus Algorithm (RPCA)|Fast and low-cost transactions|Ripple Transaction Protocol (custom)|Cross-border payments, remittances
EOSIO|Delegated Proof of Stake (DPoS)|High throughput and low latency|C++|Decentralized applications, social media
MaalChain|Maal Validator DAO (PoA)|High TPS (Upto 4000)|Go|Decentralized Applications, Concept of Identity-based Private dApps

### Ethereum
![ethereum](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/82929c4a-89d1-448a-8212-3ed2de0faf98)

Ethereum: Launched in 2015 by Vitalik Buterin and developers, Ethereum facilitates decentralized application (dApp) and smart contract deployment.

Proof of Work (PoW) to Proof of Stake (PoS) Transition: Originally on PoW, Ethereum is transitioning to PoS with Ethereum 2.0 to enhance scalability, energy efficiency, and security.

Ethereum 2.0 Features: Ethereum 2.0, or Eth2/Serenity, addresses scalability with PoS, shard chains, and the Beacon Chain, aiming to increase transaction throughput, reduce fees, and energy consumption.

Solidity: Ethereum's primary smart contract programming language, Solidity, resembles JavaScript and C++, enabling developers to define rules and logic for self-executing agreements on the blockchain.

General-Purpose Blockchain: Ethereum supports diverse dApps beyond transactions, including decentralized finance (DeFi), non-fungible tokens (NFTs), and decentralized autonomous organizations (DAOs), fostering innovation in the blockchain space.
### Bitcoin
![bitcoin](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/c26f93da-d3c6-44f4-9b63-1ad6e03157b6)

Bitcoin's Introduction: Introduced in 2008 by Satoshi Nakamoto, Bitcoin is the first and most renowned cryptocurrency, operating on a decentralized peer-to-peer network.

Proof of Work (PoW): Bitcoin's consensus mechanism relies on PoW, where miners validate transactions by solving cryptographic puzzles, ensuring network security and immutability.

Scalability Challenges: Bitcoin faces scalability issues due to its block size limit and transaction processing time, leading to congestion and increased fees during periods of high transaction volume.

Transaction Processing Time: Bitcoin transactions can take minutes to hours to be confirmed and added to the blockchain, with an average block time of approximately 10 minutes.

Bitcoin Script: Bitcoin Script is a scripting language defining spending conditions for bitcoins, enabling smart contracts for various transactions, though less powerful than other smart contract languages.

Peer-to-Peer Digital Currency: Bitcoin serves primarily as a peer-to-peer digital currency, facilitating value transfer between users pseudonymously, recorded on the public ledger blockchain maintained by network nodes

### MaalChain
![maalchain](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/d942cbe2-885f-4dd5-8492-6056e0932048)

MaalChain Overview: MaalChain is a blockchain project emphasizing decentralized applications (dApps) and high transaction throughput, aiming to facilitate various applications, particularly focusing on identity-based private dApps.

High Transaction Throughput (TPS): MaalChain is capable of handling up to 4000 transactions per second (TPS), crucial for applications requiring fast transaction processing and scalability.

Maal Validator DAO (Proof of Authority): Operating on a Proof of Authority (PoA) consensus mechanism, MaalChain validates transactions through approved validators, potentially leading to faster confirmations and increased scalability compared to PoW systems.

Go Programming Language: MaalChain is developed using Go, known for its efficiency and scalability, making it suitable for building high-performance blockchain systems.

Decentralized Applications (dApps): MaalChain supports the development and deployment of dApps, allowing developers to leverage its high TPS and identity-based features for various applications.

Identity-based Private dApps: MaalChain's unique feature is its focus on identity-based private dApps, offering tools and mechanisms for applications prioritizing user identity management and privacy. These dApps may include features such as user authentication, access control, and data encryption to enhance user privacy and security.

