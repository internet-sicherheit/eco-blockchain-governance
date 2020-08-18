# eBGF RFC 0006: Node Software Requirements
- Authors: [Kevin Wittek](wittek@internet-sicherheit.de)
- Status: PROPOSED
- Since: 2020-08-12
- Status Note: Implemented by Sovrin to a certain degree
- Start Date: 2020-08-12
- Tags: 

## Summary

Software requirements for operating a blockchain node.
This applies to application-level software as well as the OS layer.

## Motivation

While a blockchain system can mostly be described as a heterogenous network, 
and a certain degree of heterogeneity can even be a desired property with regards to resilience,
a certain baseline should be required in order to operate a stable, production-grade, network.

Though it might be technically possible to operate a blockchain network without specifying software requirements,
it might be challenging to offer it in a business context while guaranteeing certain SLAs.

By implementing this RFC it is demonstrated, that a conscious decision about the software involved with operating the node and with regards to non-functional operative quality attributes has been made.

## Specification

An implementation should consider the following topics (with the list not being exhaustive):

* OS and OS version
* Server OS hardening
  * Enable and configure hardening modules (e.g. SELinux, AppArmor)
* Versions of critical system libraries
* Application version
  * Docker image tag
  * deb/rpm package version
* Limiting installed software packages on the node to those required to operate the node software
* Usage and configuration of OS-level software firewall

## Examples & Best Practices

We can look at the [Sovrin Steward Technical and Orgnaizatoinal Policies](https://sovrin.org/wp-content/uploads/Steward-Technical-and-Organizational-Policies-V2.pdf) as an example implementation:

> * If a Node is run on a VM, the Steward:
>   * MUST run on a mainstream hypervisor that receives timely patches from its vendor or community.
>   * SHOULD apply hypervisor patches on a regular basis.
> * The Node MUST run in an OS that is dedicated to the validator, i.e., a single-purpose (physical or virtual) machine that MUST run Sovrin Open Source Code, MAY run other software approved by the TGB, and MUST NOT run any other software. Software required to support the node, such as monitoring, backup, and configuration management software, are approved as a general category. However, Stewards should discuss with the TGB any software packages that transmit between the Steward Node and the outside.
> * MUST run a server with compatible versions of the operating systems supported by the Hyperledger Indy Node requirements as documented in the release notes.
> * MUST have a system clock that is demonstrably in sync with well-known NTP servers.


## Drawbacks

Having certain requirements might exclude potential node operators for joining the network.
This could mean that the requirements don't fit their existing software policies (which might make operation impossible or increase operational costs), or that the requirements come withe software license costs 

In addition, the requirements ensure a certain degree of homogeneity.
While we mentioned this as a desired property in the motivation, this also brings the danger, that certain attacks might become applicable to all nodes of the network.

## Prior art

The [Sovrin Governance Framework](https://sovrin.org/library/sovrin-governance-framework/) defines software requirements to a certain degree as part of the [Steward Technical and Orgnaizatoinal Policies](https://sovrin.org/wp-content/uploads/Steward-Technical-and-Organizational-Policies-V2.pdf).

[bloxberg]() provides some rough requirements as part of the [bloxbergValidatorSetup installation instructions](https://github.com/bloxberg-org/bloxbergValidatorSetup).
However, this is mostly targeted at helping the operator getting the node up and running and is not concerning network stability.

## Unresolved questions

* Defined process for updating the software requirements.
This could potentially be handled as an RFC in the [governance](/governance) working group.
* How should this RFC be implemented, if there are different classes of nodes?
* Other software-related topics, such as monitoring, alerting, backups, etc. shall be defined in another RFC.