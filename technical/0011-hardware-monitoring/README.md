# 0011: Hardware monitoring
 - Authors: [Iosif Peterfi](peterfi@mpdl.mpg.de), [David Maas](david_maas@hotmail.de), [Chinmay Khandekar](khandekar@internet-sicherheit.de), [Kevin Wittek](wittek@internet-sicherheit.de) 
- Status: [PROPOSED](/README.md#proposed)
- Since: 2020-10-21 
- Status Note: Initial Proposal  
- Start Date: 2020-10-21 
- Tags: monitoring, operational, performance, status, nodes

## Summary
Describes hardware monitoring and monitoring the status of node uptime and performance status.

## Motivation
Due to the decentralized nature of the blockchain infrastructure, it is challenging to find an appropriate method for monitoring the status of all running nodes. 

Validating if a node is running or not is insufficient to determine the overall health of a specific node. 

Once adequate measures have been taken to properly monitor a node's performance, then a overall network health can be determined.

## Specification
The following parameters are prerequisites for effective hardware monitoring:
* Selection of the components to be monitored
* Selection of the measured variables
* Selection of sensor technology
* Definition of sampling rates
* Selection of the transmission protocols
* Monitoring of the operating system
* Monitoring the hard disk(s)
* Monitoring of external storage units
* Monitoring RAID systems
* Monitoring server ventilation / cooling
* Monitoring working memory (RAM)
* Monitoring system voltage
* Monitoring Uninterruptible power supply (UPS)
* Use of a hardware watchdog
* Selection of the detection method
* Display of the measured values
* Selection of the analysis method
* Selection of the visualisation technology
* Selection of the alarm method
* Use of early detection 

The following factors have to be determined for each core node
* Connectivity to node software
* CPU available/used
* Memory available/used
* Disk available/used
* Bandwidth available/used
* Transaction propagation
* Block processing time
* Link Speed

## Examples & Best Practices

Core nodes are different for each blockchain infrastructure architecture.

[Ethereum Public Network](https://github.com/ethereum/go-ethereum)
For public ethereum nodes, the bootnodes are the core nodes, as described in the documentation.

The way the Ethereum team monitors their bootnodes has been addressed by Péter Szilágyi at Devcon 5 [Monitoring an Ethereum infrastructure](https://www.youtube.com/watch?v=2I_Cfr-OUp4)
The video describes monitoring at infrastructure layer. Péter mentions they used DataDog, Graphana, Phrometheus and InfluxDB.

The PoW mining nodes can also be monitored individually by each node owner.

[European Blockchain Services Infrastructure](https://ec.europa.eu/cefdigital/wiki/display/CEFDIGITAL/EBSI)

A mixture of various monitoring tools are used apparently by EBSI to [monitor the infrastructure layer](https://ec.europa.eu/cefdigital/wiki/display/CEFDIGITALEBSI/Monitoring+of+the+Infrastructure) . One tool being mentioned is [phpservermon](https://github.com/phpservermon/phpservermon)
For the blockchain layer, this service category is mentioned in EBSI V1, however it [may contain further monitoring tools](https://ec.europa.eu/cefdigital/wiki/display/CEFDIGITALEBSI/Blockchain+Monitoring). As of V1, the existing monitoring tools are block explorers.


Finding an appropriate way of monitoring the infrastrucutre layer is challenging and is highly depended on the infrastructure architecture. Security considerations have to be taken into account when the core nodes are owned and controlled by various parties.

The blockchain layer monitoring can be easily adapted from a working solution if the underlying blockchain technology is the same (ie: Ethereum based blockhain)

## Drawbacks

Monitoring the infrastructure layer introduces overhead caused by reporting processes.

Monitoring the blockchain layer required a big amount of resources. The process involves parsing the blockchain and creating a regular database with the parsed information. This may use 10 times more disk space as the blockchain itself uses. Disk, CPU and Memory requirements for monitoring the blockchain layer grows toghether with the blockchain disk footprint.

## Prior art

Further information can be found at [Hyperledger Besu Monitor Metrics](https://besu.hyperledger.org/en/stable/HowTo/Monitor/Metrics/)

## Unresolved questions

* Defining a process to ingest and visualize the data reported by the core nodes 
* Defining a process for reporting hardware resource available and usage
* How to report the information needed for monitoring without granting more permissions that are required to perform the tasks.
* Establishing an alerting strategy when multiple node owners are involved
