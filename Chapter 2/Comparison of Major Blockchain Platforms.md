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

### Blockchain
- chain that verified a block of transaction data
- decentralized with Peer-2-Peer technology directly, intermediate race

### Bitcoin?
- introduced in 2008 by an anonymous person or group using the pseudonym Satoshi Nakamoto
- decentralized peer-to-peer network
- multiple copies of data (DLT)

Proof of Work (PoW): Bitcoin operates on a Proof of Work consensus mechanism. This means that transactions on the network are validated and added to the blockchain by miners solving complex cryptographic puzzles. Miners compete to solve these puzzles, and the first one to solve it gets to add a new block of transactions to the blockchain and receives a reward in the form of newly created bitcoins. PoW ensures the security and immutability of the Bitcoin network.

Limited Scalability: Bitcoin's scalability refers to its ability to handle a large number of transactions quickly and efficiently. However, Bitcoin faces challenges in scalability due to its block size limit and the time it takes to process transactions. As a result, the network can become congested during periods of high transaction volume, leading to delays and increased transaction fees.

Slower Transaction Processing: Transactions on the Bitcoin network can take several minutes to several hours to be confirmed and added to the blockchain. This is due to the time it takes for miners to validate transactions and add them to a new block. Bitcoin's block time, or the average time it takes to mine a new block, is around 10 minutes.

Bitcoin Script: Bitcoin Script is a simple scripting language used to define the conditions under which bitcoins can be spent. It allows users to create customizable smart contracts and execute various types of transactions. While Bitcoin Script is not as powerful as some other smart contract languages, it still enables a wide range of use cases, such as multi-signature wallets and time-locked transactions.

Peer-to-Peer Digital Currency: Bitcoin is primarily used as a peer-to-peer digital currency for transferring value between users. Transactions are recorded on a public ledger called the blockchain, which is maintained by a network of nodes running the Bitcoin software. Bitcoin transactions are pseudonymous, meaning that while transaction details are publicly available, the identities of the parties involved are not directly tied to their Bitcoin addresses.

### MaalChain

#### What is MaalChain
MaalChain is a blockchain project that aims to provide a decentralized platform for various applications, particularly focusing on high transaction throughput and identity-based private decentralized applications (dApps). Here's an overview of its key features and components:


High Transaction Throughput (TPS): MaalChain boasts high transaction throughput, with the capability of handling up to 4000 transactions per second (TPS). High TPS is a crucial feature for blockchain networks, especially for applications that require fast transaction processing and scalability.

#### MaalChain Consensus Mechanism
Maal Validator DAO (Proof of Authority): The MaalChain network operates on a Proof of Authority (PoA) consensus mechanism. In a PoA system, transactions are validated by a set of approved validators rather than a decentralized network of miners. This can contribute to faster transaction confirmations and increased scalability compared to Proof of Work (PoW) systems.

Go Programming Language: MaalChain is developed using the Go programming language. Go is known for its efficiency and scalability, making it a suitable choice for building high-performance blockchain systems.

Decentralized Applications (dApps): MaalChain supports the development and deployment of decentralized applications (dApps). These are applications that run on a blockchain network and are not controlled by any single entity. Developers can build various types of dApps on MaalChain, leveraging its high TPS and identity-based features.

Identity-based Private dApps: One of the distinctive features of MaalChain is its focus on identity-based private dApps. This implies that the platform provides tools and mechanisms for building applications that prioritize user identity management and privacy. Identity-based dApps may offer features such as user authentication, access control, and data encryption to ensure the privacy and security of user information.

