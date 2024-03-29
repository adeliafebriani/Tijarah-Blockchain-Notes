# Digital Signatures

![Digital-signature](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/2ce4b82e-34be-4c74-9f7d-357c695f876d)

> [!NOTE]
> The private key is retained by the signor and anyone else will receive the public key which allows anyone to review the signed document.

### Digital Signatures
A digital signature is a handwritten signature or a stamped seal but with far more inherent security built into its design. It is a mathematical scheme for demonstrating the authenticity of digital messages or documents.

### Technical Mechanism
![digital sign](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/1673b113-4db1-4c05-ad5a-ea0fb288e5c0)

1. Creation of Digital Signatures:
   * A digital signature is created using a private key to 'sign' a transaction or a piece of data.
   * When users initiate a blockchain transaction, they generate a digital signature using their private key.
   * This process involves creating a hash of the transaction data and then encrypting the hash with the private key.
2. Verification Process:
   * The verification of a digital signature is done using the signer’s public key.
   * When other participants in the blockchain network receive the transaction, they use the sender's public key to decrypt the signature. They independently compute the hash of the original transaction data. If this hash matches the decrypted hash from the signature, it confirms that the transaction is authentic and has not been tampered with.

### Key Properties of Digital Signatures in Blockchain
![Screenshot 2024-03-21 140256](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/fe16d7b8-2334-4ca8-9b5c-6ccf1ec96cf8)

1. Integrity: Digital signatures ensure the integrity of a transaction by certifying that the contents have not been altered in transit.
2. Authentication: They provide proof of the origin of the transaction, affirming that the stated sender indeed created it.
3. Non-repudiation: The signer cannot deny their intention of the transaction since the digital signature uniquely binds them to it.
4. Security: Digital signatures are virtually impossible to forge, provided the private key remains secure.

### Applications in Blockchain
1. Transaction Verification:
   * Signed by the sender’s private key and verified by the network, ensuring that the rightful owner of the digital assets initiates the transaction.
2. Smart Contracts:
   * Ethereum, digital signatures are used to execute smart contracts, ensuring that the contract is executed by the parties involved without repudiation.
3. Identity Verification:
   * Require identity management to use digital signatures to authenticate user actions and secure personal data.

### Security Considerations
The security of a digital signature in blockchain is tied to the security of the private key. If a private key is compromised, it can lead to unauthorized transactions and breaches. Therefore, robust key management practices are essential.
