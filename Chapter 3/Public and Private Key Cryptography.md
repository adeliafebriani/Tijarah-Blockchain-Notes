# Public and Private Key Cryptography
### Basic Principles
1. Key Pair: public key=shared openly, private key=kept secret.
2. Encryption and Decryption: Messages encrypted=public key, decrypted=private key, and vice versa.
3. Digital Signatures: Anyone using a public key can verify data signed with the private key.

### Technical Details
1. Key Generation:
   * Asymmetric cryptography relies on algorithms that generate keys based on mathematical problems with no efficient solving methods
   * Eg: the factoring of large prime numbers (RSA algorithm) & the discrete logarithm problem (as in ECC - Elliptic Curve Cryptography).
2. Encryption Process:
   * Data encryption involves mathematical algorithms that use the public key to transform data into a format that can only be reversed (decrypted) with the corresponding private key.
3. Signature Creation and Verification:
   * A digital signature is created by processing the data with a private key, and its authenticity can be verified using the corresponding public key.

### Elliptic Curve Cryptography (ECC)
![ecc graph](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/dfd45b1b-3481-46a1-ab3e-4471f2f12f56)

ECC is a public-key cryptography technique that uses elliptic curves to generate security for key pairs.

### Difference between Private Key and Public Key
|Private|Public key|
|:---:|:---:|
|+Faster|-Slower|
|Same key (secret key) used to encrypt and decrypt the message|Two keys which one key is used for encryption, and the other is used for decryption|
|The key is kept a secret|One of the two keys is kept a secret|
|Symmetrical (one key)|Asymmetrical (private & public)|
|+used for large amounts of text|-used for only short messages|
|-the possibility of losing the key that renders the systems void|+less possibility of key loss, as the key is held publicly|
|Can be shared between two parties|Can be used by anyone|
|Performance testing checks the reliability, scalability, and speed of the system.|Load testing checks the sustainability of the system.|
|The private key is used in algorithms such as AES 128, AES 192 and AES 256.|The public key is used in algorithms such as RSA, DSA, etc.|
|The private key is kept secret.|The public key is widely distributed.|
|It is used to protect disk drives and other data storage devices.|It is used to secure web sessions and emails.|
|The recipient’s private key decrypts the message.|The recipient’s public key encrypts the message.|
|If the private key is the locking key, then the system can be used to verify documents sent by the holder of the private key.|If the public key is the locking key, then it can be used to send private communication.|

### Public Key Infrastructure (PKI)
![public key](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/cf2ff186-bc46-4f27-ad14-a8a211885c84)

* PKI is roles, policies, hardware, software, and procedures to create, manage, distribute, use, store, and revoke digital certificates.
* Plays a crucial role in managing public key encryption.
* A digital certificate, issued by a Certificate Authority (CA), ensuring the public key's authenticity.

#### Certificate Authority (CA)
![ca](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/21aa193d-953f-4c55-bf26-280edf3d5758)

* Responsible for issuing
* Revoking
* Distributed digital certificate
* Often a trusted third-party organization

### Applications in Blockchain
1. Transaction Verification:
   * A user's public key is their address, while the private key is used to sign transactions.
   * Only the private key owner can authorize transactions from their account.
2. Security and Anonymity:
   * While the public key is visible to all participants in the blockchain network, the private key remains confidential, maintaining security and user anonymity.

### Security Considerations
1. Key Management:
   * The security of asymmetric cryptography heavily relies on how private keys are managed and stored.
   * The system's security is at risk if a private key is compromised.
2. Computational Power:
   * The security of public and private key cryptography is based on the current limitations of computational power and algorithmic efficiency.
   * It is essential to stay updated with cryptographic advancements to counteract potential future vulnerabilities, such as those posed by quantum computing.

> [!NOTE]
> * Public and private key cryptography is a cornerstone of digital security.
> * It enables secure, confidential, and authenticated transactions over insecure channels like the Internet.
> * Its application in blockchain technology ensures the security and integrity of transactions and forms the basis of trust in these decentralized systems.
> * Understanding the technical intricacies of this cryptographic method is essential for appreciating its role in securing digital communications and transactions in the modern digital era.
