# 0007: Different node types and classes
- Authors: [David Maas](david_maas@hotmail.de), [Mirko Mollik](mollik@trustcerts.de) 
- Status: PROPOSED
- Since: 2020-09-09 
- Status Note: Initial Proposal  
- Start Date: 2020-09-09 
- Tags: 

## Summary

Describes the different types and classes of nodes.

## Motivation

To operate a Blockchain network it is important to know the different node types and classes and to use them correctly.

There are several ways to operate a node. To get an overview of all possible ways. 

Dividing nodes and members in different types and classes allows to use design patterns like [principle of least privilege](https://en.wikipedia.org/wiki/Principle_of_least_privilege) or efficient ressource handling.

## Specification

The following is an overview of the different types and classes of a node (the list is not exhaustive):

Types:
- Full Node
- Light Node
- Service Node

Classes:
- Validator Node
- Observer Node
- Other Node
- Bootnode


## Examples & Best Practices

The [ethereum documentation](https://ethereum.org/en/developers/docs/nodes-and-clients/) can serve as an example for the types of nodes.

> If you want to run your own node, you should understand that there are different types of node that consume data differently. In fact, clients can run 3 different types of node - light, full and archive. There are also options of different sync strategies which enables faster synchronization time. Synchronization refers to how quickly it can get the most up-to-date information on Ethereum's state.

>  Full node
 - Stores full blockchain data.
 - Participates in block validation, verifies all blocks and states.
 - All states can be derived from a full node.
 - Serves the network and provides data on request.
 
> Light node
- Stores the header chain and requests everything else.
- Can verify the validity of the data against the state roots in the block headers.
- Useful for low capacity devices, such as embedded devices or mobile phones, which can't afford to store gigabytes of blockchain data.

> Archive node
- Stores everything kept in the full node and builds an archive of historical states. Needed if you want to query something like an account balance at block #4,000,000.
- These data represent units of terabytes which makes archive nodes less attractive for average users but can be handy for services like block explorers, wallet vendors, and chain analytics.
> Syncing clients in any mode other than archive will result in pruned blockchain data. This means, there is no archive of all historical state but the full node is able to build them on demand.

We can look at the [Sovrin Steward Technical and Orgnaizatoinal Policies](https://sovrin.org/wp-content/uploads/Steward-Technical-and-Organizational-Policies-V2.pdf) as an example implementation for node classes:
> A Steward Node:
> * MUST be available to run as a Validator Node or Observer Node on any of the formal ledgers that make up the Sovrin Network.

We can also take a look at the [Hyperledger Besu documentation](https://besu.hyperledger.org/en/stable/HowTo/Find-and-Connect/Bootnodes/) as an example of the use of bootnodes: 
> Using Bootnodes is a method for initially discovering peers. Bootnodes are regular nodes used to discover other nodes.

> Bootnodes and static nodes are parallel methods for finding peers. Depending on your use case, you can use only bootnodes, only static nodes, or both bootnodes and statics nodes. For example, you run multiple nodes on MainNet (discovery using bootnodes), but want to ensure your nodes are always connected (using static nodes).

## Drawbacks

There is too much fragmentation in the types and classes of nodes. There is no standard implementation because most blockchains are desiged for a special use case (running dapps for public usage or offering a registry for self sovring identities in public or private networks) but all projects are oriented towards the technology. This makes it very cluttered.

## Prior art

 Sovrin provide frameworks and technical documentation that define Node requirements. 
 [Steward Technical and Orgnaizatoinal Policies](https://sovrin.org/wp-content/uploads/Steward-Technical-and-Organizational-Policies-V2.pdf)
 [Hyperledger Besu](https://besu.hyperledger.org/en/stable/) and [Ethereum](https://ethereum.org/en/developers/docs/) each provide technical documentation.

## Unresolved questions

Standardisation of the types and classes of nodes and the related compatibility of the block chain as a whole. 
