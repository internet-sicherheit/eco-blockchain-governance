# eco Governance Framework

Based on the Sovrin Governance Framework, a governance framework for Blockchain technology is being developed. The Sovrin Steward Technical and Organizational Policies V2 were used and analysed and adapted for the eco Governance Framework. Subsequently, of course, also extended.

---

## General Security Policies

First the questions are extracted from the guidelines and then examples of implementation are given.

 1. What does a secure organizational structure look like and how do you implement it?
 2. How to ensure continuous safe operation?
 3. How do you regulate security for administrative staff?
 4. How do you ensure the ongoing operation and integrity of your employees?
 5. What are the physical security requirements?
 6. What are the security requirements for outsourcing to a third-party provider?
 7. How is compliance with this Directive ensured for the operator?
 
___
 
 1. Security policies and practices must be defined and provided in order to operate a steward. This includes all services    related to the operation of the steward and the staff involved. An employee must be appointed to supervise the correct operation. This includes reviewing and updating the guidelines and, in addition to training employees, enforcing the guidelines.
 2. The safety guidelines must be reviewed at least once a year to ensure safe operation.
 3. Administrative staff pose a high security risk. Accordingly, they must be reviewed regularly. This process must be initiated for new recruits and repeated regularly. This also applies to administrative employees of subsidiaries who are involved in the operation. This includes, among other things, proof of identity, police clearance certificates and other security measures that the operator considers necessary, provided that these are compatible with the law.
 4. Employees who are involved in the services provided must regularly attend training courses on security and data protection. This should be done at least once a year and an agreement should be reached which guarantees ethical behaviour in particular and also deals responsibly with confidentiality, security, data protection and privacy. In addition, tailored training and guidelines must be provided for employees who have administrative access to subcomponents. 
 5. If the nodes are operated in their own premises, it must be ensured that the guidelines also guarantee physical security and access control and that the best possible industry standards are adhered to.
 6. If the nodes are hosted by a third-party provider, the operator must ensure that the security, privacy and data security policies of the third-party provider meet the requirements of this document. 
 7. The operator must provide an inspection body on request with evidence of compliance with the guidelines and all accreditations. In particular certificates, attestations or reports from accredited third parties. This includes standards such as ISO 27001, SSAE SOC 2 and others. 

---

## General Node Policies

 1. Availability and type of nodes?
 2. Operation of the node? (software)
 3. Software update window?
 4. Updating the node configuration?
 5. Number of employees required to operate the node?
 6. Accessibility of the administrators?
 7. Time window for recovery after error or system failure?

___

 1. The nodes must be available as validation nodes or observation nodes in the network.
 2. The node must run software specified by the Technical Board.
 3. The software must be updated within 3 working days after the Technical Board has made a recommendation and a competent management entity confirms this by vote.
 4. The configuration for the network must be transmitted to the required location in good time. To this end, the information must be updated within 3 working days in the event of changes. 
 5. At least 2 IT-qualified employees must be responsible for the node as administrators. In addition, there must be another employee with access and sufficient qualifications to manage the node in an emergency. Imaginable scenarios are, attacks or when the network can not create consensus. 
 6. Contact information must be provided by all administrators. These are reviewed quarterly. 
 7. Backups, snapshots or images must be kept available so that a recovery after an error is possible within one hour or less.

---

## Node Technical Policies

The guidelines apply to the production network. A test network should implement these guidelines. 

 1. Minimum requirements of the hardware class?
 2. Using and updating virtual machines?
 3. Minimum requirement of the software?
 4. Compatibility with certain network standards?
 5. Hardware requirement CPU?
 6. Hardware requirement RAM?
 7. Hardware requirement main memory? (hard drive)
 8. Connection to the Internet?
 9. Network requirements?
 10. Ensuring the high availability of the node?
 11. Reliable synchronization of the system time?
 12. Securing the power supply?

___
 
 1. The node must run on server hardware.
 2. If the node is running on a virtual machine, make sure to use a virtualization that is regularly updated by the vendor or a community and these updates must be performed regularly.  
 3. The node must run on an operating system that is intended for the validator. (Single-purpose physical or virtual machine) It shall run software specified by the Technical Board, and may also use software released by the Technical Board. No other software may be run on the machine. Software that is used for configuration, backup and monitoring is permitted. However, all software packages that are transferred between the nodes and the outside world should be discussed with the technical board. 
 4. Must run a server that provides a compatible operating system for network, according to the specifications of the network.  
 5. Must have adequate computing power. (16 cores or more)
 6. Must have sufficient memory. ( 64 GB or more )
 7. Must have at least 2 TB of storage with the option to grow to 4 TB. For example via Raid implementations. The start partition must also be sufficiently large.
 8. Must have a high-speed connection to the Internet with highly available, fail-safe lines. 1 Gbps 
 9. Must provide at least one dedicated NIC for consensus traffic and have another NIC to handle external requests. Each NIC must have a stable, static, globally routable IP address.
 10. Nodes must be implemented in such a way that the high-availability architecture is not compromised. Implementation of the node selection algorithm so that the individual nodes do not take on more responsibility than intended. So that a recovery reacts to errors within a reasonable time. 
 11. A system clock is required that has been proven to be synchronized with known NTP servers.
 12. A power supply is required that meets the requirements of a high-availability system.
 

---

## Node Security Policies

 1. How to ensure authentication and authorization of the stewards and nodes in the network?
 2. How can it be certified that the nodes are running in a secure environment?
 3. How is the separation of public and internal systems regulated?
 4. Possibilities of remote maintenance?
 5. Realization of the access control?
 6. Update intervals of nodes and internal systems?
 7. Regulation of access control over the network?
 8. Authorization of the nodes in the network?
 9. Ensuring the ongoing integrity of the systems?

___

 1. The steward keys must be managed on a different system than the system on which the nodes run. A possible implementation would be via a "CLI (Command Line Interface) System". Thus, nodes in the network can be authorized and stewards authenticated. For this possible CLI system no high end hardware is required. However, best IT security practices must be used for nodes that meet or exceed the following guidelines. 
 2. It must be ensured and certified that the node is operated in a secure data center. Including appropriate security levels and specifications at which they are targeted. For example, compliance with SSAE 16 Type II or other standards.
 3. The nodes must not run on the same system as the internal systems of the stewards. This serves to protect the internal systems because the nodes are publicly visible. 
 4. It must be ensured that a current state of the art technology is used for remote access to the nodes and internal systems. (At least SSH with key plus password plus source IP firewall rule and two-factor authentication wherever possible)
 5. It must be ensured that only the assigned administrators have access to the nodes and CLI systems, whether remote or local.
 6. The latest updates must be installed within a week or less. The time limit should be as short as possible. (24 hours or less)
 7. It must be certified that the server on which the node is running is protected by a firewall. Furthermore, it must be ensured that no public access is possible, except on ports required for the node software. It must be ensured that only administrators from outside can access the systems. The output ports should also be blocked to ensure that no jumps are made from one node to another.
 8. A security audit tool must be carried out and the results subsequently submitted to the Technical Board. After approval, the node can participate in the consensus procedure. 
 9. The security clearance tool shall be run from time to time as requested by the Technical Board and shall deliver the results within 3 working days.
 

---

## Node Operating Policies

 1. How can the alarm be implemented redundantly in the event of faults? 
 2. Regulation of downtime?
 3. Network-wide planning of downtime?

___

 1. The operator must provide 2 technical contact points responsible for managing the node with an SMS-capable device for alerting.
 2. The operator should aim for 99,9 % uptime for the nodes. (This corresponds to about 1.4 minutes of downtime per day or 9 hours per year).
 3. It should coordinate with other operators in advance a downtime together with the technical board. Everything should be settled amicably.


---

## Node selection algorithm

 1. Application of the node selection algorithm?
 2. Manual adjustments of the node selection algorithm?
 3. Design of the node selection algorithm?
 4. How is the node selection algorithm made transparent and public?
 
 ___

 1. Active Validator nodes must be determined in the production network by the node selection algorithm defined by the Technical Board.
 2. Non-technical inputs or policy decisions implemented by the node selection algorithm MUST be approved by the Technical Board.
 3. At all times, the node selection algorithm must represent the best efforts of the Technical Board to design an algorithm that applies the basic principles of the eco Governance Framework. In recognition of the inherent tensions and trade-offs between some of the basic principles, priority should be given to balancing when designing this algorithm: 
 The principles of Decentralization by Design, especially the principles of diffuse trust and high availability. 
 The principles of Security by Design, especially the principles of system diversity and secure failure.
 4. A human readable, understandable and explainable description of the current draft of the algorithm as approved by the Technical Board SHALL be published by the Technical Board in the official repository and made publicly available through a web page.


---

## Permissioned Test Network Policies

 1. What configurations are possible in the permissioned test network? 
 2. How is access to the permissioned test network possible?
 3. Who can become a transaction endorser for the Permissioned Test Network?
 4. What happens if personal data is found in the Permissioned Test Network?

___

 1. Via the Permissioned Test Network
The steward must serve at least one node, but can serve more than one node. Any number of nodes can be hosted as hosting providers at the steward's discretion. It is not necessary to execute the node selection algorithm.
 2. Any access to the Permissioned Test Network must be controlled by Permissioned Write Access (note that this does not allow writing personal data).
 3. To be a transactional endorser for the Permissioned Test Network, an organization must either:
Be a member of eco.
Be a steward of the permissioned test network.
Be a steward-authorized transaction support in the permissioned est network.
 4. If at any time, for any reason, personal information is discovered on the Permissioned Test Network:
A supervisory body must be notified immediately.
Within 48 hours of notification, the Control Panel must reset the Permissioned Test Network to delete the personal data.

---

## Reporting Policies

 1. How are changes to the operator to be communicated? 
 
 ___

 1. An operator shall report any significant change in the configuration or location of a node to the competent governance body within 5 working days of the change.
