# Proof of Stake
Proof of Stake (PoS) is an alternative to Proof of Work (PoW). It aims to achieve distributed consensus while **addressing some of the inefficiencies of PoW**, particularly its high energy consumption.

### Fundamentals of Proof of Stake

* **Staking**: Unlike PoW, where miners solve cryptographic puzzles, PoS requires network participants (validators) to 'stake' their cryptocurrency as collateral to validate transactions and create new blocks.

* PoS uses an election process in which 1 node is randomly chosen
![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/f3fd0a2f-ba05-490a-b989-86d5f85fe3be)

* **Validator Selection**: Validators are selected to create a new block based on various factors, including the amount of cryptocurrency they hold and are willing to lock up (stake), and the length of time they have held it.

* To become a validator, a node has to deposit a certain amount of coins into the network as a stake (security deposit). Size of the stake = chances of a validator.
![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/5701025f-5177-470a-940c-8179d7ba0574)

### How Proof of Stake Works

* **Creating a New Block**: In PoS, a validator is chosen to create a new block based on a random selection process influenced by their stake. The larger their stake, the higher the chance of being selected.

* **Validating Transactions**: Once a validator creates a block, other validators will verify the transactions within the block. If deemed valid, the block is added to the blockchain.

* **Rewards**: Validators are rewarded for their efforts in validating transactions, typically with transaction fees or network-specific rewards.

* Creating new block >>> validate transaction >>> rewards

### Technical Aspects of PoS

* **Randomization**: The process of selecting validators is pseudo-random but generally weighted towards those with larger stakes and longer holding times.

* **Security**: The security in PoS comes from the requirement for validators to lock up their tokens. Acting maliciously could lead to losing their stake or being expelled from the network.

* **Slashing**: Many PoS systems implement a 'slashing' mechanism where a validator’s stake can be partially or fully slashed if they are found to be acting dishonestly.

### Advantages and Challenges 

Advantages | Challenges
--- | ---
**Energy Efficiency**: PoS is far more energy-efficient than PoW, eliminating the need for intensive computational work | **Nothing at Stake Problem**: PoS systems may face unique security challenges like the "nothing at stake" problem, where validators might have incentives to validate multiple blockchain histories, potentially leading to network instability.
**Reduced Centralization Risk**: The PoS mechanism can mitigate the risk of centralization seen in PoW, where miners with significant computational power can dominate the process. | **Initial Distribution**: The initial distribution of coins can affect network security. If a few participants hold large amounts of the currency, it could centralize control.

### PoW vs PoS

PoW = Miners vs PoS = Validators
![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/e4d703b3-aabb-4c85-90bd-65bcfa33eb38)

PoW's node stakes are more expensive vs. approved or work-based.
![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/b263100d-f753-47e6-932e-a09adb220f32)
