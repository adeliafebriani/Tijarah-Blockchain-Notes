# Cryptographic Hash Function
### What is  a cryptographic hash function?
![cryptographic-hash-functions-means](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/3b8c358d-2322-4f48-9b61-902f50932048)

An algorithm that takes (input=message) and returns a fixed-size string of bytes (output=hash/digest) that represent the input data.

![block](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/fb443c60-7d58-498e-ae29-dd4737e88743)

A hash function is designed to secure and manage data integrity.

### Core Properties
![Screenshot 2024-03-19 133147](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/431a2332-7ead-49f2-9a99-775c07b5b8eb)

1. Deterministic: The same input will always produce the same hash output.

![Screenshot 2024-03-19 133336](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/22c4a349-991c-4896-92d9-75abb87a8c7f)

2. Quick Computation: The hash function can process any size of the data quickly and return a hash value in a consistent time frame.

> [!Note]
> Most computers can compute million/second hash

3. Small Changes Lead to Significant Differences: A tiny change in input data will produce an entirely different hash (avalanche effect).

![single-character-changes-hash-algorithm](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/2ac38c04-0a9e-44d7-aa71-3c8c4cb92aa6)

4. Pre-image Resistance (one way): It is computationally unfeasible to reverse-engineer the original input from its hash output and infeasible to reconstruct the original input data. This property is important for securing data and making it tamper-evident.

![Screenshot 2024-03-25 154617](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/3bdbe5bc-f6d3-48e4-87b2-e97f38dd8e09)
   
5. Second Preimage Resistance (weak collision resistance): It is computationally infeasible to find any second input which has the same output as any specified input.

![Screenshot 2024-03-25 154639](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/29cf1c70-e157-4394-97ef-c789cc28c5cc)

6. Collision Resistance (strong collision resistance): It is computationally infeasible to find any two different inputs hash to the same output, nearly impossible and crucial for data integrity.

![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/00731330-2863-4b67-a166-d4dd7b4a30af)


### Technical Details
![Screenshot 2024-03-19 133028](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/5a473b38-83f7-4127-b436-1f381aa8e72e)

1. Hash Size
   * The length of the hash output is critical
   * SHA-256, produces a 256-bit (32-byte) output
   * The size ensures a vast range of possible hash values, contributing to collision resistance
2. Algorithm Structure:
   * message padding (to ensure that the input data is of a certain length)
   * breaking the input into blocks
   * processing these blocks through a series of mathematical operations

### Applications in Blockchain
1. Creating Block Hashes
   * Each block has a unique hash- created from the block's data (including the previous block's hash)
   * Any alteration in the block data changes its hash, affecting the entire chain
   * Ensuring data integrity
2. Mining and Proof of Work
   * Cryptographic hashes are central to mining in Proof of Work-based blockchains like Bitcoin.
   * Miners must find a hash that is below a certain target, which requires computational work, thereby securing the network through energy and computational commitment.

> [!NOTE]
> * Cryptographic hash functions are vital in ensuring the security and integrity of data in various digital applications.
> * Their ability to provide a secure, one-way, and collision-resistant method of encoding information is fundamental.
> * Appreciating how cryptographic hash functions underpin the security of modern digital transactions and data management systems.
