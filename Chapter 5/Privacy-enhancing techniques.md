# Privacy-Enhancing Techniques 
Privacy-enhancing techniques are methods or strategies employed to protect individuals' personal information and mitigate the risks associated with unauthorized access, surveillance, or misuse. Here are some common privacy-enhancing techniques:

### Encryption
![encryption_keys](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/1ecd0f08-13bc-422e-820b-ccf33178670c)

As mentioned earlier, encryption involves encoding data in such a way that only authorized parties can decrypt and access it. This ensures that even if data is intercepted, it remains unreadable to unauthorized individuals.

### Pseudonymization
Similar to anonymization, pseudonymization involves replacing or masking personally identifiable information with pseudonyms or codes. This allows for data analysis while reducing the risk of directly identifying individuals.

### Anonymization
![Pseudonymization vs Anonymization Key Differences](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/eff6fddc-3b4e-437d-81ad-b4d7d658523b)

Anonymization techniques remove or obscure personally identifiable information (PII) from datasets, making it challenging to link data to specific individuals. This protects individuals' privacy while still allowing for data analysis and utilization.

### Data Minimization
![data min](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/4855c325-f04c-45be-9e96-c2373deae761)

Data minimization involves collecting and retaining only the minimum amount of personal data necessary for a specific purpose. Reducing the amount of data collected and stored minimises the risk of privacy breaches.

### Access Controls
![access control](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/9ab7f9f0-4d33-4b36-a04e-dace90344a92)

Implementing access controls ensures that only authorized individuals have access to personal data. This includes user authentication, role-based access control, and encryption of data at rest and in transit.

### Privacy by Design
![Privacy-by-Design](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/f0b85685-bc94-4872-bdda-67a51537789a)

Privacy by design is a system and product development approach that prioritizes privacy and data protection from the outset. It involves incorporating privacy-enhancing features and practices into the design and development process.

### User Consent and Transparency
Providing clear information to users about data collection, processing, and sharing practices, and obtaining their informed consent is essential for respecting individuals' privacy rights.

### De-identification Techniques
De-identification involves removing or obscuring identifying information from datasets to protect privacy while allowing data analysis and sharing.

De-identification is the process of removing or hiding explicit identifiers from data so that the remaining information cannot identify an individual. De-identification techniques include:
* Generalizing: Replacing specific values with a broad range or category
* Suppression: Replacing or removing sensitive values entirely
* K-anonymity: Grouping data to hide unit-level records that relate to specific individuals
* Differential privacy: Adding random noise to a dataset to mask the impact that any one record can have on the outcome
* Aggregation: Combining data from multiple individuals to create groups or cohorts, thereby making it difficult or impossible to identify specific individuals within the dataset

### Privacy-Enhancing Technologies (PETs)
PETs encompass a range of technologies designed to protect individuals' privacy, including secure communication protocols, anonymity networks, and privacy-focused browsers and tools.

### Differential Privacy
Differential privacy is a rigorous privacy framework that aims to protect individuals' sensitive information while still allowing for meaningful data analysis. It involves adding noise or randomness to query responses to prevent the re-identification of individuals in datasets.

### Zero-Knowledge Proofs
Zero-knowledge proofs are a fascinating cryptographic technique that allows one party (the prover) to prove to another party (the verifier) that a statement is true without revealing any additional information beyond the validity of the statement itself. In essence, the prover convinces the verifier that they possess certain knowledge or information without actually disclosing what that knowledge is.

#### How Zero-Knowledge Proofs Work:
Let's say Alice wants to prove to Bob that she knows the solution to a complex mathematical problem without revealing the solution itself. They agree on a protocol for zero-knowledge proof:

1. Commitment: Alice commits to a solution without revealing it. She could, for example, encrypt the solution and send it to Bob.
2. Challenge: Bob selects a random challenge, such as asking Alice to prove that her solution satisfies a specific property.
3. Response: Alice responds to the challenge based on her knowledge of the solution. This response convinces Bob that she indeed knows the solution without revealing what it is.
4. Verification: Bob verifies the response using the commitment and challenge, confirming that Alice's response is valid according to the agreed-upon rules.

If Alice completes this process multiple times for different challenges, Bob becomes increasingly convinced that Alice does possess the knowledge she claims to have.

> [!NOTE]
> Zero-knowledge proofs allow parties to interact and exchange information while minimizing the risk of exposing sensitive data.
