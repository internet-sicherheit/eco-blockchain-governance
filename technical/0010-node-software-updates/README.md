# 0010: Node software updates
- Authors: [David Maas](david_maas@hotmail.de), [Mirko Mollik](mollik@trustcerts.de) 
- Status: PROPOSED
- Since: 2020-09-09
- Status Note: Initial Proposal
- Start Date: 2020-09-09
- Tags:

## Summary

Software update policy for operating a blockchain node. This applies not only to the applications but also to the operating system. 

## Motivation

To create a safe environment throughout the blockchain network, software update guidelines are extremely important. All nodes must be updated at a certain interval to ensure safe operation. However, the actual process is quite complex as the entire network must be considered.

## Specification

- Update protocol
- Versioning
- Minor updates without interrupting the network 
- Major updates should be planned
- Guaranteed availability of the system

## Examples & Best Practices

Based on the version system there could be different protocols to update a node. If the software of the blockchain nodes follows the [semantic versioning](https://semver.org/) protocol, MINOR and PATCH updates should be updatable without breaking the network functionality. For major patches a coordinated update has to be planned and can lead to a short downtime of the network because of a change in the communication protocol.

Beside the current node version the uptime of the system has to be guaranteed. An uncoordinated process can lead to a nonfunctional consensus.

We can look at the [Sovrin Steward Technical and Orgnaizatoinal Policies](https://sovrin.org/wp-content/uploads/Steward-Technical-and-Organizational-Policies-V2.pdf) as an example implementation:
> A Steward Node:
> * MUST run a release of the Sovrin Open Source Code as approved and designated by
    the Technical Governance Board (TGB).
> * MUST facilitate an upgrade to a new version of the Sovrin Open Source Code within
    three (3) business days of a new release that has been: a) recommended by the Sovrin
    TGB, and b) accepted by a vote of any other relevant Sovrin Governing Body (such as
    the Steward Council).

A clear and strict protocol has to be defined to avoid accidents like the [Überlingen mid-air collision](https://en.wikipedia.org/wiki/2002_%C3%9Cberlingen_mid-air_collision) where the involved parties followed different suggestions.

## Drawbacks

Some update policies like blue-green can lower the security level. In this case the private key has to be shared between the current running system and a new one will replace it on the fly. Securing the wallet in a dedicated module with an API will make the node more complex, but allow the usage of a blue-green based protocol.

Based on the update policy and the release schedule of the blockchain software the amount of updates can increase. If the update process cannot be automated as much as possible, too much interaction is required which can lead to human errors.

Without checking the changes of the update the risk of new injected malicious code that can steal the wallet or even delete the chains on all nodes exists. So only versions verified by a trusted party should be used.

## Prior art

 Sovrin provide frameworks and technical documentation that define Node requirements. 
 [Steward Technical and Orgnaizatoinal Policies](https://sovrin.org/wp-content/uploads/Steward-Technical-and-Organizational-Policies-V2.pdf)

## Unresolved questions

A software update process with standardised guidelines for blockchain projects. A de facto standard for all blockchain technologies to ensure more security and simplification. 
