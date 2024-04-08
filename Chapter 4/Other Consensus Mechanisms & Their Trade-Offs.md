# Other Consensus Mechanisms & Their Trade-Offs

## Proof of Authority (PoA)
![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/937c509b-d30b-420b-9cf7-8f2407f78716)

Proof of Authority (PoA) represents a consensus  algorithm that is based on reputation, creating a practical and efficient solution for blockchain networks, especially when it comes to private ones.

![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/c5910fd0-d666-4aab-8b13-1754bc947a66)

The main form of leverage in PoA is  none other than a user’s identity, a block validator isn’t staking  coins, but their very own reputation.

This means that PoA blockchains are secured by the validating nodes that are randomly chosen to serve as trustworthy entities.

![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/4dbe85ad-20a1-49c2-ac61-9d34b57ef2bc)

PoA uses a limited number of block validators,  which makes the system highly scalable. Both blocks and transactions are verified by pre-approved participants, who serve as moderators of the system.

### What Benefits Does Proof of Authority Have?

Unlike PoW, and similar to PoS,  PoA doesn’t rely on solving puzzles in order to make sure that there is a continuous connection between nodes. PoA validator doesn’t require special equipment to help maintain the network. It is great for reducing  the amount of power used.

PoA also enjoys a greater speed for validating transactions. Blocks are generated in a predictable sequence by taking into consideration the number of validators, which means that the blockchain will enjoy a higher transaction rate when compared to PoW or PoS.

![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/8faf8f9a-6367-471b-8af4-ac07e191e365)

PoA also stands out thanks to its resistance to 51% attacks. That is because it is incredibly hard to get control over 51% of authorities that aren’t connected directly.

Nodes are pre-authenticated, so, in the case that one is not available, the network can remove it from the validation process. 

### What Downside Does Proof of Authority Have?

![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/c8f43291-6856-4fac-a313-3cbcaf1b4e33)

Just like PoW or PoS, PoA  also has its limitations. Since validators need to be verified, trusted, and picked by the network, this translates into having a rather small validating group. This does offer the benefit of a higher level of throughput, but it also makes a PoA network more centralized.

![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/a09c793f-78c9-4799-9832-a74177dc4462)

Because block rewards are visible  to everyone in a public blockchain, anyone can see how much a certain PoA validator has earned. This means that there may be a higher risk of corruption or manipulation. 

![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/b183d68c-4eaf-41d4-a73b-74d279af0c2d)

This is why the validator needs  to be an entity that is trusted. Becoming a validator is also rather hard as candidates need to pass a notary exam  which attests to no criminal record and the good moral standing of a candidate while also  filtering out those who aren’t committed.

Then again, the result does  translate into a pro for PoA, but, to get there, it may turn  many people off from trying.

### Can It Be Used In A Decentralized Manner?

The PoA mechanism works best in a centralized  way, due to the reasons such as having a small number of validators. 

This means that many believe PoA to be a consensus mechanism that aims to make centralized systems better  and more efficient, not decentralized ones.

The PoA can be used in corporations that have high  logistical needs, but within the crypto community, it is very unlikely that it would be embraced in its current form.

### Trade-offs

Trade-Off|Proof of Authority (PoA)
---|---
Decentralization vs. Efficiency	|Prioritizes efficiency over decentralization, with a limited number of trusted validators.
Security vs. Speed	|Offers fast transaction finality, but security relies heavily on the integrity of trusted validators.
Permissioned vs. Permissionless|	Typically permissioned, requiring participants to be granted permission to become validators or join the network.
Resistance to Sybil Attacks	|Resistant to Sybil attacks due to known validators but susceptible to attacks or collusion by those validators.

### Conclusion

![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/8ba68b97-c976-4394-8ffa-26d9f9206bf9)

Proof of Authority is a consensus mechanism that stands out for relying on a validator’s  reputation to make the blockchain work properly.

While it’s a more environmentally friendly  method than PoW, and it is faster, the network will always be limited by  the small number of validators active, and by the fact that, by design, it can’t  be used in a decentralized manner - for now.

## Proof of Elapsed Time (PoET)

![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/6feaad1d-5b00-4a19-8dfa-a3084149e4b9)

Proof of Elapsed Time (PoET) is a consensus algorithm primarily designed for permissioned blockchains and is developed by Intel and is based on the Trusted Execution Environments (TEEs) provided by Intel's Software Guard Extensions (SGX) technology.

In PoET, nodes compete to generate a random wait time, and the node that  completes the wait time first is chosen to create the next block. To ensure that nodes don't cheat by generating shorter wait times, PoET uses special hardware called trusted execution environments (or TEEs) that create a random wait time and protect it from manipulation.

PoET is a more efficient and environmentally friendly consensus algorithm than traditional proof of work because it doesn't require nodes to perform complex mathematical  calculations. Instead, PoET relies on the random wait time generated by the TEEs.

### Key Principle

The key principle behind PoET is that it leverages the security guarantees provided by SGX enclaves to ensure fairness and randomness in the selection of block creators. Since the wait time is generated within the enclave and cannot be tampered with, PoET helps to prevent centralization and manipulation in blockchain networks.

PoET has been used in various blockchain platforms, including Hyperledger Sawtooth and some enterprise blockchain solutions. However, it's worth noting that PoET has also faced criticisms, particularly regarding its reliance on SGX technology and concerns about the centralization of trusted sources providing wait times.

### Difference Between Proof of Work and Proof of Elapsed Time

Feature|Proof of Work (PoW)|Proof of Elapsed Time (PoET)
---|---|---
Consensus Mechanism|Requires miners to solve complex puzzles.|Participants request a wait time from a trusted source.
Selection Process|	Competitive: Miner who solves puzzle first wins.|	Lottery-based: Participant with shortest wait time wins.
Resource Intensive|	Requires significant computational power and energy.|	Less resource-intensive as it doesn't involve mining.
Security|	Provides strong security through computational puzzles.|	Relies on trusted execution environments for security.
Energy Efficiency|	Known for its high energy consumption.|	More energy-efficient as it doesn't involve continuous mining.
Example|	Bitcoin, Ethereum (currently transitioning to PoS).|	Hyperledger Sawtooth.
