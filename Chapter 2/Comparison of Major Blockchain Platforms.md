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

Ethereum is a decentralized blockchain platform launched in 2015 by Vitalik Buterin and other developers. It is designed to enable developers to build and deploy decentralized applications (dApps) and smart contracts.

Proof of Work (PoW) and Transitioning to Proof of Stake (PoS): Initially, Ethereum operated on a Proof of Work consensus mechanism, similar to Bitcoin, where miners validate transactions and add them to the blockchain. However, Ethereum is in the process of transitioning to a Proof of Stake (PoS) consensus mechanism with the Ethereum 2.0 upgrade. PoS relies on validators who lock up a certain amount of Ether as a stake to validate transactions and create new blocks. This transition aims to improve scalability, energy efficiency, and security on the Ethereum network.

Working on Ethereum 2.0 for Improved Scalability: Ethereum 2.0, also known as Eth2 or Serenity, is a major upgrade to the Ethereum network aimed at addressing scalability issues. It introduces several key features, including the switch to PoS, shard chains to improve network throughput, and the Beacon Chain, which serves as the backbone of the new PoS consensus mechanism. Ethereum 2.0 aims to significantly increase the number of transactions the network can process while reducing fees and energy consumption.

Solidity: Solidity is the primary programming language used to write smart contracts on the Ethereum platform. It is a statically typed, contract-oriented language with syntax similar to JavaScript and C++. Solidity allows developers to define the rules and logic of smart contracts, which are self-executing agreements stored on the blockchain. Smart contracts enable a wide range of applications, including decentralized finance (DeFi), non-fungible tokens (NFTs), and decentralized autonomous organizations (DAOs).

General-Purpose Blockchain, Decentralized Applications: Ethereum is often referred to as a general-purpose blockchain because it supports the development of a wide range of decentralized applications beyond simple peer-to-peer transactions. These applications, known as dApps, leverage Ethereum's smart contract functionality to create various decentralized services, such as decentralized exchanges, lending platforms, gaming applications, and more. Ethereum's open and programmable nature has made it a popular platform for innovation in the blockchain space.

### Bitcoin
![bitcoin](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/c26f93da-d3c6-44f4-9b63-1ad6e03157b6)

Bitcoin is the first and most well-known cryptocurrency, introduced in 2008 by an anonymous person or group using the pseudonym Satoshi Nakamoto. It operates on a decentralized peer-to-peer network, allowing users to transact directly with one another without the need for intermediaries like banks.

Proof of Work (PoW): Bitcoin operates on a Proof of Work consensus mechanism. This means that transactions on the network are validated and added to the blockchain by miners solving complex cryptographic puzzles. Miners compete to solve these puzzles, and the first one to solve it gets to add a new block of transactions to the blockchain and receive a reward in the form of newly created bitcoins. PoW ensures the security and immutability of the Bitcoin network.

Limited Scalability: Bitcoin's scalability refers to its ability to handle a large number of transactions quickly and efficiently. However, Bitcoin faces challenges in scalability due to its block size limit and the time it takes to process transactions. As a result, the network can become congested during periods of high transaction volume, leading to delays and increased transaction fees.

Slower Transaction Processing: Transactions on the Bitcoin network can take several minutes to several hours to be confirmed and added to the blockchain. This is due to the time it takes for miners to validate transactions and add them to a new block. Bitcoin's block time, or the average time it takes to mine a new block, is around 10 minutes.

Bitcoin Script: Bitcoin Script is a simple scripting language used to define the conditions under which bitcoins can be spent. It allows users to create customizable smart contracts and execute various types of transactions. While Bitcoin Script is not as powerful as some other smart contract languages, it still enables a wide range of use cases, such as multi-signature wallets and time-locked transactions.

Peer-to-Peer Digital Currency: Bitcoin is primarily used as a peer-to-peer digital currency for transferring value between users. Transactions are recorded on a public ledger called the blockchain, which is maintained by a network of nodes running the Bitcoin software. Bitcoin transactions are pseudonymous, meaning that while transaction details are publicly available, the identities of the parties involved are not directly tied to their Bitcoin addresses.

### MaalChain
![maalchain](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/d942cbe2-885f-4dd5-8492-6056e0932048)

MaalChain is a blockchain project that aims to provide a decentralized platform for various applications, particularly focusing on high transaction throughput and identity-based private decentralized applications (dApps). Here's an overview of its key features and components:

High Transaction Throughput (TPS): MaalChain boasts high transaction throughput, with the capability of handling up to 4000 transactions per second (TPS). High TPS is a crucial feature for blockchain networks, especially for applications that require fast transaction processing and scalability.

Maal Validator DAO (Proof of Authority): The MaalChain network operates on a Proof of Authority (PoA) consensus mechanism. In a PoA system, transactions are validated by a set of approved validators rather than a decentralized network of miners. This can contribute to faster transaction confirmations and increased scalability compared to Proof of Work (PoW) systems.

Go Programming Language: MaalChain is developed using the Go programming language. Go is known for its efficiency and scalability, making it a suitable choice for building high-performance blockchain systems.

Decentralized Applications (dApps): MaalChain supports the development and deployment of decentralized applications (dApps). These are applications that run on a blockchain network and are not controlled by any single entity. Developers can build various types of dApps on MaalChain, leveraging its high TPS and identity-based features.

Identity-based Private dApps: One of the distinctive features of MaalChain is its focus on identity-based private dApps. This implies that the platform provides tools and mechanisms for building applications that prioritize user identity management and privacy. Identity-based dApps may offer features such as user authentication, access control, and data encryption to ensure the privacy and security of user information.

