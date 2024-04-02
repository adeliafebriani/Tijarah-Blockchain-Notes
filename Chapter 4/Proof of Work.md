# Proof of Work
![pow](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/4336b1d8-1449-46bf-99f5-a22363d5f842)

Proof of Work (PoW) is one of the consensus mechanisms role in securing networks like Bitcoin. 

### Fundamentals of Proof of Work

* **Concept**: Miners compete to solve a complex problem that requires computational resources. The first to solve the problem gets the opportunity to add a new block of transactions to the blockchain and is rewarded.

* **Cryptographic Puzzle**: The core of PoW is a cryptographic puzzle, often a hash function, where miners must find a value (nonce) that, when hashed with the block data, produces a hash output that meets specific criteria (like a certain number of leading zeroes).
Technical Mechanics of PoW

* **The Puzzle**: The puzzle in PoW is designed to be difficult to solve but easy to verify. This typically involves performing a hash function repeatedly, altering the nonce each time, until the output meets the network's criteria.

* **Difficulty Adjustment**: The difficulty of the puzzle can be adjusted. For instance, in Bitcoin, the difficulty adjusts every 2016 block to ensure that a new block is added approximately every 10 minutes, regardless of the total computational power in the network.

* **Block Reward**: Miners are incentivized to participate in the process through block rewards, which include newly minted coins and transaction fees.

### Security and Decentralization

* **Network Security**: The computational effort required to solve the puzzle protects the network from attacks. To alter any block, an attacker would need to redo the work for that block and all subsequent blocks, which is practically infeasible due to the high computational cost.

* **Decentralization**: PoW promotes decentralization since it allows anyone with the necessary computational resources to participate in the mining process.

### Challenges and Criticisms

* **Energy Consumption**: PoW is often criticized for its high energy consumption, as miners consume significant electrical power to perform the necessary calculations.

* **Centralization of Mining Power**: There is a concern that large-scale mining operations with more resources could dominate the process, potentially centralizing control.

* **Scalability**: PoW can lead to slower transaction processing times and higher fees, especially as the network grows.