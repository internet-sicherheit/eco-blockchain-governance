# 0005: Node Hardware Requirements
- Authors: [David Maas](david_maas@hotmail.de), [Kevin Wittek](wittek@internet-sicherheit.de), [Chinmay Khandekar](khandekar@internet-sicherheit.de) 
- Status: PROPOSED
- Since: 2020-08-12 
- Status Note: Initial Proposal  
- Start Date: 2020-08-12 
- Tags: 

## Summary

Describes the hardware requirements for the node.

## Motivation

For the node to run optimally, certain requirements should be placed on the hardware. 
This is the only way to ensure that there is as little downtime as possible and that there are sufficient resources available in the network.

## Specification

A realization of the hardware should consider the following points (the list is not exhaustive):

- The node can run on dedicated server hardware or inside a server cluster
- When running inside a sever cluster, the resources have to be dedicated to the node
- Must have adequate computing power.
- Must have sufficient memory.
- Must have sufficient storage with the option to expand it.  
- Must have a high-speed connection to the Internet.
- Must have an IP address allocated. This IP address must be reachable by other nodes.
- Enough electricity must be supplied to the hardware to be able to function at highest capacity. 

## Examples & Best Practices

We can look at the [Sovrin Steward Technical and Orgnaizatoinal Policies](https://sovrin.org/wp-content/uploads/Steward-Technical-and-Organizational-Policies-V2.pdf) as an example implementation:

> * MUST run on robust server-class hardware.
> * MUST have adequate compute power (in late 2019, 8 or more cores is considered adequate).
> * MUST have adequate RAM (in late 2019, 32 GB of RAM is considered adequate).
> * MUST have at least 1 TB, with the ability to grow to 2 TB, of reliable (e.g., RAIDed) disk space, with an adequately sized boot partition.
> * MUST have a high-speed connection to the internet with highly available, redundant pipes (as of late 2019, 100 Mbps was considered adequate).
> * MUST have at least one dedicated NIC for Sovrin Validator Node consensus traffic, and a different NIC to process external requests. Each NIC must have astable, static, world-routable IP address.
> * SHOULD have a power supply consistent with high availability systems. 

There is also a possible implementation by EBSI [Minimum Requirements for Hosting an EBSI v1.0 Node](https://ec.europa.eu/cefdigital/wiki/display/CEFDIGITALEBSI/Minimum+Requirements+for+Hosting+an+EBSI+v1.0+Node)

European Blockchain Services Infrastructure (EBSI)

> Requirements
>
> Environment Requirements
>
> An EBSI v1.0 node requires a minimum of three computer hosts all with access to the Internet and with individual fixed public IP addresses. These can be either physical server computers or virtual machines running in a self-hosted data-centre infrastructure, a private cloud, or a public cloud.
>
> Hardware
>
> Each computer host – physical or virtual – must have these minimum specifications:
> * 4 Core CPU, 4 vCPU or equivalent,
> * 16 GB of RAM for the BESU and Fabric hosts; 32 GB of RAM for Master/Applications host
> * 80 GB SSD,
> * 256 GB SSD.
>
> Network
>
> All hosts must be in the same subnet, each with a fixed public IP address, and must be connected to the Internet in order to get updated and to communicate with other EBSI nodes. 
>
> The minimum specifications are:
> * 1 GB Ethernet (local network),
> * latency 50ms (internet),
> * 100 Mbits/second for bandwidth (internet)
> * 3 fixed public IPs (one for each host).

The bloxberg blockchain is another example 

bloxberg: Blockchain Infrastructure for Scientific Research

> Pilot Phase [bloxberg Whitepaper 1.0](https://www.mpg.de/13416733/bloxberg_whitepaper.pdf)
>
> Minimum specifications - physical or virtual - for a validator node are:
> * 1 Core CPU
> * 1GB of RAM 
> * 4 GB Storage
>
> Current Phase [bloxberg ValidatorSetup](https://github.com/bloxberg-org/bloxbergValidatorSetup)
>
> Minimum specifications - physical or virtual - for a validator node are:
> * 2 Core CPU
> * 2GB of RAM
> * 100 GB Storage SSD

It is important to note that the requirements specified in the example implementation need to be adapted according to the network's context. 

## Drawbacks

High costs for hardware and operation could exclude potential members. 
It would be much cheaper to operate nodes privately without guidelines. 
However, this would also result in the loss of collateral. 
Presumably the consequence would be more failures. 
In addition, the overall trust would also be lost. 

## Prior art

The EU and Sovrin provide frameworks and technical documentation that define hardware requirements. 
[EBSI Technical Documentation](https://ec.europa.eu/cefdigital/wiki/display/CEFDIGITALEBSI/Technical+Documentation) and [Steward Technical and Orgnaizatoinal Policies](https://sovrin.org/wp-content/uploads/Steward-Technical-and-Organizational-Policies-V2.pdf)

## Unresolved questions

- A constant adaptation of the requirements would still have to be regulated in order to ensure operation in the future. 
This should be clarified in another RFC.
