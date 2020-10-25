# 0008: Used consensus algorithm
- Authors: [David Maas](david_maas@hotmail.de) 
- Status: PROPOSED
- Since: 2020-10-21 
- Status Note: Initial Proposal  
- Start Date: 2020-10-21 
- Tags: 

## Summary
Describes the consensus method used Algorithm.

## Motivation
Consensus procedures are a crucial element of any block chain network as they ensure that the integrity and security of these decentralised systems are maintained.

## Specification
The following consensus algorithms are available:

* Proof of Work
* Proof of stake
* Proof of authority (PoA)
* Proof of Importance 
* Practical Byzantine Fault Tolerance (PBFT) 


## Examples & Best Practices
We can look at the Sovrin Steward Technical and Orgnaizatoinal Policies as an example implementation:
> Node Selection Algorithm
>1. The selection of active Validator Nodes at any point in time, at least on the Sovrin Main
Network, MUST be governed by the Node Selection Algorithm as specified by the Sovrin
TGB.
>2. Non-technical inputs or policy decisions implemented by the Node Selection Algorithm
MUST be approved by the Sovrin Board of Trustees.
>3. At any point in time, the Node Selection Algorithm MUST represent the TGB’s best
efforts at designing an algorithm that applies the Core Principles of the Sovrin
Governance Framework. Recognizing the inherent tension and tradeoffs between some
of the Core Principles, the design of this algorithm should give priority to balancing:
>a. The Decentralization by Design principles, in particular the principles of Diffuse
Trust and High Availability.
>b. The Security by Design principles, in particular the principles of System Diversity
and Secure Failure.
>4. A human-readable, understandable, and explainable description of the current design of
the algorithm as approved by the TGB MUST be published by the TGB in the official
Sovrin Code Repository and made publicly visible via a web page on the Sovrin
Foundation website.

>[Hyperledger Besu](https://besu.hyperledger.org/en/stable/Concepts/Consensus-Protocols/Overview-Consensus/) implements the following consensus protocols:

>* Ethash (Proof of Work)
>* Clique (Proof of Authority)
>* IBFT 2.0 (Proof of Authority)
>* Quorum IBFT 1.0 (Proof of Authority).

>Comparing Proof of Authority consensus protocols
Besu implements the Clique and IBFT 2.0 Proof of Authority consensus protocols. Proof of Authority consensus protocols work when participants know each other and there is a level of trust between them. For example, in a permissioned consortium network.

>Proof of Authority consensus protocols have faster block times and a much greater transaction throughput than the Ethash Proof of Work consensus protocol used on the Ethereum MainNet.

>In Clique and IBFT 2.0, a group of nodes in the network act as signers (Clique) or validators (IBFT 2.0). The existing nodes in the signer/validator pool vote to add nodes to or remove nodes from the pool.

## Drawbacks
Depending on the chosen algorithm there are pros and cons. There is no algorithm that achieves the best performance in every respect.

## Prior art
Sovrin provide frameworks and technical documentation that define Node requirements. [Steward Technical and Orgnaizatoinal Policies](https://sovrin.org/wp-content/uploads/Steward-Technical-and-Organizational-Policies-V2.pdf)
Hyperledger Besu implements various consensus algorithms [Overview-Consensus](https://besu.hyperledger.org/en/stable/Concepts/Consensus-Protocols/Overview-Consensus/)

## Unresolved questions
* How can/should the algorithm be optimized?
* When and how will the algorithm be run?
* How will results of the algorithm be used to adjust network configuration?