# Consensus Mechanisms in Blockchain
![Consensus Mechanism](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/f5f2f495-ca79-4d86-a45d-9b738c3deb42)

Consensus Mechanisms are the protocols that 
- ensure all nodes in a blockchain network agree on the validity of transactions
- maintaining the integrity and trust in the distributed ledger

Without it,
- lack of synchronization and agreement among nodes
- leading to potential conflicts
- security issues

### Why Are Consensus Mechanisms Necessary?

1. **Decentralization**: CM enables network participants to agree on the current state of the ledger. 

2. **Security**: Protect the blockchain from fraudulent transactions and malicious actors. By requiring agreement from multiple nodes, it's hard to make any single entity manipulate the ledger.

3. **Integrity and Trust**: CM ensures that once a transaction is confirmed, it can be trusted as valid. This builds confidence among users in the system's reliability.

4. **Network Synchronization**: Ensuring every participant has the same, up-to-date version of the ledger.

## Consensus Mechanisms

Proof of Work (PoW)|Proof of Stake (PoS)|Delegated Proof of Stake (DPoS)|Proof of Authority (PoA)|Proof of Elapsed Time (PoET)
:---:|:---:|:---:|:---:|:---:
Bitcoin, Ethereum (currently), and others.|Ethereum (upcoming Ethereum 2.0), Cardano, and more.|EOS, Tron, and others.|Private or consortium blockchains where high throughput and scalability are needed.|Intel’s Sawtooth platform.
Nodes (miners) solve complex mathematical puzzles to validate transactions and create new blocks.|Validators are chosen to create new blocks based on the number of coins they hold and are willing to 'stake' as collateral.|A variant of PoS where stakeholders vote for a few delegates who manage the blockchain on their behalf.|Nodes are validated and selected as trustworthy entities.|Randomizes the process of electing block creators using a fair lottery system.
The first to solve the puzzle gets the right to add the block to the blockchain and is rewarded.|More energy-efficient than PoW and offers faster transaction processing.|Offers scalability and efficiency but can be less decentralized.|Less decentralized, relying on the reputation of the validators.|Energy-efficient and suitable for permissioned blockchain networks.
PoW is secure but energy-intensive and can lead to scalability issues.|Favor wealthier nodes with more significant stakes.|||

## Byzantine Fault Tolerance (BFT)

BFT is a system property that can resist the cause of failure from Byzantine problems.
> [!NOTE]
> BFT will continue operating even when some of the node fails to communicate

buy bitcoin-pow
protocol-validation transaction

## Istanbul Byzantine Fault Tolerance (IBFT)
![IBFT](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/e0a34003-832d-4dde-a0f5-13a97125414a)

IBFT adapts the Byzantine Fault Tolerance (BFT) mechanism designed to work in Ethereum-based blockchain systems.

#### How it works?

* **Validator Nodes**: A group of validator nodes is pre-determined. They are responsible for managing the consensus process.

* **Block Validation Process**: Block created, and propagated to the validator nodes. For the block to be validated and added to the blockchain, a supermajority (typically more than two-thirds) of the validator must agree on its validity.

* **Fault Tolerance**: IBFT can tolerate up to 1/3 of the validator nodes acting maliciously or going offline without affecting the network's integrity and performance.

* **Finality**: Once a block is confirmed, it cannot be changed or reversed, eliminating the possibility of forks.

#### Advantages
* provides quick and final consensus with high fault tolerance.
* suitable for permissioned or consortium blockchains where validators are known and trusted entities.

## Practical Byzantine Fault Tolerance (PBFT)
PBFT was introduced to address the limitations of the traditional Byzantine Fault Tolerance in practical, real-world applications.

#### How it Works?

* **Three-Phase Protocol**: PBFT operates in three phases - pre-prepare, prepare, and commit. This ensures that all nodes in the network agree on the new block's content.

* **Leader Selection**: One node is elected as the leader (primary), which proposes the block. Other nodes (replicas) validate and agree on the proposed block.

* **Fault Tolerance**: Like IBFT, PBFT can handle up to 1/3 of faulty nodes in the network.

#### Advantages
* efficient and offers a low-latency consensus mechanism without intensive computational requirements
* ideal for networks where participants are partially trusted
* a high transaction throughput is necessary

#### Use Cases
PBFT is commonly used in private or consortium blockchain networks, particularly where quick consensus and transaction finality are important.
