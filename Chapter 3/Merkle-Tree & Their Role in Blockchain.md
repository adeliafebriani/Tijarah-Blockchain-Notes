# Merkle-Tree & Their Role in Blockchain
### What is a Merkle Tree?
![tree](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/d67eead0-0fea-4d30-96b8-7e4eb80d674a)

A Merkle tree is a binary tree of hashes.
* At the bottom layer (leaf nodes)
* Each node represents the hash of a block of data (e.g., a transaction in the blockchain).
* Each non-leaf node is a hash of its two child nodes.
* This structure continues until there is a single hash at the top of the tree, known as the Merkle root.
* The Merkle root is a concise representation of the integrity of all the underlying data.

### Technical Mechanics

Creating a Merkle Tree:

Hashing Each Piece of Data: Each piece of data (like a transaction in the blockchain) is hashed using a cryptographic hash function.

Pairing and Hashing Upwards: These hashes are then paired and hashed together, and the process continues upwards until a single hash remains — the Merkle root.

Verifying Data Using Merkle Trees:

To verify the integrity of any single piece of data, you don’t need to download the entire blockchain. Instead, you only need the smallest chain of hashes linking your piece to the Merkle root.

This chain of hashes, along with the Merkle root, can prove whether the piece of data is indeed part of the tree without revealing the entire dataset.

### Role in Blockchain

Efficiency in Data Verification: Merkle trees allow for efficient and secure verification of large datasets common in blockchain. They enable quick and lightweight verification of whether a specific transaction is included in a block.

Security and Integrity: By structurally incorporating cryptographic hashing, Merkle trees help ensure the integrity of the blockchain data. Any alteration in a transaction would require recomputation of all subsequent hashes up to the Merkle root, which is computationally impractical.

Scalability: For blockchains, especially those with high transaction volumes, Merkle trees offer a way to scale efficiently. They reduce the amount of data needed to be transmitted, stored, and processed when verifying transactions.

### Technical Considerations

Hash Function: The choice of the hash function is critical for the security of the Merkle tree. Functions like SHA-256 (used in Bitcoin) provide a good balance of speed and security.

Tree Structure: While binary trees are common, some implementations may use different structures (like a Patricia tree in Ethereum) for specific optimization purposes.

### Conclusion

Merkle trees are a fundamental component in the architecture of blockchain technology. They provide an efficient means of summarizing and verifying large datasets, a necessity in the world of distributed ledger technologies. Their use in blockchain is a testament to the elegant solutions cryptography can offer to complex problems in data integrity and verification, making them an indispensable element in the secure and efficient operation of blockchain networks.
