# 0016: Automated verification of node compliance
- Authors: [David Maas](david_maas@hotmail.de), [Mirko Mollik](mollik@trustcerts.de) 
- Status: PROPOSED
- Since: 2020-09-09 
- Status Note: Initial Proposal  
- Start Date: 2020-09-09 
- Tags: 

## Summary
Describes the automatic verification of nodes with a specific compliance.

## Motivation
To operate a safe environment at all times, it is important that the nodes meet certain requirements. 
Since a manual process would be too time-consuming, automation of Verified Nodes is very important. 
Thereby any compliance should be defined.

## Specification
To enable verification, the following points would have to be present:
* Compliance guidelines
* Observer
* Verification routines
* Time interval of the repetition

## Examples & Best Practices
[Hyperledger Fabric](https://hyperledger-fabric.readthedocs.io/en/release-2.2/policies/policies.html) provides basic ways to apply compliance to a Blockchain.

>Policies are one of the things that make Hyperledger Fabric different from other blockchains like Ethereum or Bitcoin. In those systems, transactions can be generated and validated by any node in the network. The policies that govern the network are fixed at any point in time and can only be changed using the same process that governs the code. Because Fabric is a permissioned blockchain whose users are recognized by the underlying infrastructure, those users have the ability to decide on the governance of the network before it is launched, and change the governance of a running network.

## Drawbacks
If security gaps could be exploited, automation would of course also be very dangerous.

## Prior art
Further information can be found at [Hyperledger Fabric.](https://hyperledger-fabric.readthedocs.io/en/release-2.2/)

## Unresolved questions
A way for a permission-free public Blockchain to adjust the compliance during operation without changing the code.
