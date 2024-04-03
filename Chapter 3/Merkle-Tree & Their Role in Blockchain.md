# Merkle-Tree & Their Role in Blockchain
### What is a Merkle Tree?
![tree](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/d67eead0-0fea-4d30-96b8-7e4eb80d674a)

A Merkle tree is a binary tree of hashes:
* Bottom layer = leaf nodes
* Each node represents the hash of a block of data == transaction in the blockchain.
* Each non-leaf node is a hash => two child nodes.
* It continues until a single hash at the top of the tree = Merkle root.
* The Merkle root = integrity of all the underlying data.

### Technical Mechanics
![Merkle-Tree](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/ec7be686-798e-4a65-b5e7-ed82a6532849)

1. Creating a Merkle Tree:
   * Hashing Each Piece of Data: Each piece of data (like a transaction in the blockchain) is hashed using a cryptographic hash function.
   * Pairing and Hashing Upwards: These hashes are then paired and hashed together, and the process continues upwards until a single hash remains — the Merkle root.

2. Verifying Data Using Merkle Trees:
   * To verify the integrity of any single piece of data, you only need the smallest chain of hashes linking your piece to the Merkle root.
   * This chain of hashes can prove whether the data is part of the tree without revealing the entire dataset.

### Role in Blockchain

1. **Efficiency in Data Verification**
   * Efficient and secure verification of large datasets common in blockchain.
   * Enable quick and lightweight verification of whether a specific transaction is in a block.
     
2. **Security and Integrity**
   * By structurally incorporating cryptographic hashing, Merkle trees help ensure the integrity of the blockchain data.
   * Any alteration in a transaction would require recomputation of all subsequent hashes up to the Merkle root, which is computationally impractical.

3. **Scalability**
   * High transaction volumes, Merkle trees offer a way to scale efficiently.
   * They reduce the amount of data needed to be transmitted, stored, and processed when verifying transactions.

### Technical Considerations

1. **Hash Function**
   * The choice is critical for the security of the Merkle tree.
   * Functions like SHA-256 (used in Bitcoin) provide a good balance of speed and security.

2. **Tree Structure**
   * Binary trees are common, some implementations may use different structures (like a Patricia tree in Ethereum) for specific optimization purposes.
