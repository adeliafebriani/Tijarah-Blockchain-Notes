# Practical Byzantine Fault Tolerance (PBFT)
![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/9f0e57e0-c950-45c3-9350-d9ce8798b754)

Published by Miguel Castro and Barbara Liskov in 1999, the original paper posed a solution to the Byzantine Generals' problem. Paxos and Raft aren’t by default Byzantine fault tolerant, though there are variants of them – like BFT-PaxosS. **PBFT was one of the original papers published on the topic of solving consensus when considering Byzantine faults**.

The PBFT algorithm handles less than ⅓ Byzantine faults, as we saw in the section with the Byzantine generals' problem. More traditionally, this has been written as the system can handle
f Byzantine faults, where there are 3f + 1 total nodes. It’s also really fast.

The original PBFT paper showed that when integrated with standard unreplicated NFS, a distributed file system protocol developed by Sun Microsystems in 1984, the resulting BFT-NFS is only 3% slower, although it can now withstand
Byzantine faults.

### PBFT algorithm

The main PBFT algorithm consists of three phases – pre-prepare, prepare, and commit. 

PBFT begins when the client submits a request to the primary node (Derrick). The primary node is responsible for advocating for the client's request, and this should be familiar since it’s a common design pattern. For example, remembering back to Paxos, the Proposer proposes new decrees to other legislators in the Paxon Parliament based on the requests of the people.

![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/3c0e3945-0f3c-46ac-9117-fd747794bebf)

In this case, the primary node is Derrick. We have a total of 4 nodes, meaning that we
should be able to withstand 1 fault since ¼ is less than ⅓. 

![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/aaba0db7-0f62-4c36-ba07-f00409ed5a87)

So let’s say one of our 4 nodes, Nadir, drops out due to a spotty internet connection. Nadir might’ve dropped out, but the other 3 nodes might not know that yet, so they’ll
still send messages to him.

![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/6765d2ee-1c71-4f94-9e4e-0174eee89672)

In the pre-prepare phase, the primary node Derrick sends out pre-prepare messages to everyone in the network. A node accepts the pre-prepare message so long as it's valid. 

A sequence number – like the increasing numbers Proposers in Paxos assign to each of their decrees. They also contain signatures and other useful metadata that lets nodes determine message validity.

![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/86d7753e-62fa-4364-8451-8ac7458d679a)

If a node accepts a pre-prepared message, it follows up by sending out a prepared message to everyone else. Prepare messages are accepted by receiving nodes so long as they’re valid, again, based on sequence number, signature, and other metadata. 

A node is considered “prepared” if it has seen the original request from the primary node, has pre-prepared, and has seen 2f prepare messages that match its pre-prepare – making for 2f + 1 prepares. F is the number of Byzantine faults.

![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/b2f4d78b-9939-4f2e-a49c-0b53b516cba6)

After nodes have prepared, they send out a commit message. If a node receives f + 1 valid commit messages, then they carry out the client request and then finally send out the reply to the client. 

![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/dd2fe06d-fe2c-498f-9b63-134c4cb95f5b)

The client waits for f + 1 of the same reply. Since we allow for at most f faults, we need to wait for at least f + 1, and this ensures the response is valid. After this point, the client gets the correct response. 

![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/2dcd2f6c-c1a1-4d55-863c-47d712348d38)

A diagram from the PBFT whitepaper models exactly the scenario. The diagram has five processes, or nodes in our case. The client is process C. Derrick is process 0, I’m process 1, Gloria is process 2, and Nadir is process 3.

![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/11a94c83-3e73-4ff9-b60c-651f48d08799)

In the first step, the client sent a message to Derrick, process 0. That’s the initial request. During this time, Nadir fails.

![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/1c9fad4d-baf0-4af5-b6b1-52edfd777226)

Then, Derrick sends a pre-prepared message to the rest of us processes. 

![image](https://github.com/adeliafebriani/Tijarah-Blockchain-Notes/assets/162258265/ba59e71b-fe58-4070-b997-3047e063d7ae)

Everyone except Nadir responds with a prepared message. After acknowledging everyone’s presence, we all send the commit message. After hearing a sufficient amount of commitment, we respond directly to the client.
