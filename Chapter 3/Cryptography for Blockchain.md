# Cryptography for Blockchain
### What is Cryptography?
A fundamental component of blockchain technology, providing the backbone for its security and trust mechanisms. 

> [!NOTE]
> Cryptography secure communication = information is only accessible to intended recipients. Ensure the integrity and immutability of the entire network

### Cryptographic Techniques in Blockchain
  
![hash](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/4fb22c49-7e78-4fb8-917f-44c1fdba33cb)

1. Hash Functions
   * Function: Converts input data of any size into a fixed-size string of characters, which represents the data uniquely.
   * Role: To create a unique digital fingerprint for each block and its transactions. Any alteration in the transaction data changes this fingerprint, indicating the tampering.
   * Examples: SHA-256 in Bitcoin

![public key](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/2e52f70a-dee4-497a-9753-59a0df903a94)

2. Public Key Cryptography
   * Function: Public key (shared publicly), private key (kept secret)
   * Role: To create digital signatures and for the wallet addresses in cryptocurrencies. The user will sign the transaction with a private key.
   * Security: It lies in the computational difficulty of deriving the private key from the public key.

![digital](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/ea02f2cb-4f41-416f-b686-f22586ecb815)
  
3. Digital Signatures
   * Function: Crypto technique to verify the authenticity and integrity of a message or document
   * Role:
     * A transaction created
     * It's signed digitally (use the sender's private key)
     * The sign guarantee (from a specific user) has not been altered in transit

### Importance of Cryptography in Blockchain
1. Securing Transactions: Secure encrypted and authenticated, safeguarding from fraud and unauthorized access.
2. Maintaining Integrity: The hash function maintains a continuous and unalterable chain of blocks, ensuring the integrity of the entire ledger.
3. Ensuring Anonymity and Privacy: While transactions on a blockchain are transparent, the identities of the parties involved are protected through cryptographic techniques.

> [!NOTE]
> The cryptographic principles employed in blockchain technology enable secure, transparent, and tamper-proof systems, crucial for applications ranging from cryptocurrencies to secure communication and data management.
