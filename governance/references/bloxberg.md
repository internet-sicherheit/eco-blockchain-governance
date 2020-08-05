# Bloxberg Governance Model

## Overview

The governance model is based on three pillars:

1. **Rights of co-determination**

   * Administrative rights: to propose new proposals, implement or enforce decisions

   * Control rights: ratification of decisions, follow the decision-making process and its performance
 
2. **Responsibility**: The mechanisms whereby members commit and are held accountable for their actions and decisions.

3. **incentives**: All reasons and mechanisms whereby members are encouraged to follow the guidelines

To make changes in the governance model a quorum of 75% or at least 7 organizations is required. The election takes place off-chain, typically during the summit. An amendment must receive more than 75% of the votes to be effective.


## Co-determination rights

To become a member, the organisation must meet the following criteria:
* the organisation must be active in research, for example
* have been voted by a majority of the members
 
All members have the right to initiate an off- or on-chain event.

### Decision algorithm

The decision algorithm aims to motivate the members to stick to their tasks as defined in the Governance Model.

All founding members start with a voting weight of 100, while the new members start at 0.

A vote cast on a proposal increases the voting weight, i.e.

~~~
voting weight = voting weight + 100 / (number of proposals per month)
~~~
while a missed proposal reduces the voting weight, i.e.

~~~
voting weight = voting weight - 100 / (number of proposals per month)
~~~

### New members

New members are nominated by Iron Throne every month (or every 4 weeks). The organization must fill out a form beforehand to apply for his candidacy.

The election takes place on-chain. To ratify the election, a quorum of 50% of the total voting weight must be present or at least 3 voting members.

If the candidate has received more than 50% of the vote, he is instructed to create his own node, which will be added to the network by Iron Throne.

### Iron Throne

One consortium member has the Iron Throne for one year. During this time he has the task of implementing the results of the elections, or adding new members or removing members.

The Iron Throne member organizes the Summit, a physical meeting where all members meet and make decisions.

The Iron Throne election requires a quorum of over 75% of the members or at least 3 organizations. The election takes place off-chain, or during the Summit. The organization with over 50% of the votes becomes the new Iron Throne owner.


## Responsibility
Penalties may be imposed on members who fail to comply with governance. The expulsion of a member must be approved by the other members by election.

Penalties can be triggered by the following actions:
* Node is offline for more than 3 months
* Node spams the network
* the member does not adhere to the governance model
* the member must agree to the manifesto

The exclusion of a member is done off-chain and follows the decision algorithm. A quorum of 75% is required for the election or at least 7 organizations. If more than 75% of the votes for expulsion fall, the Iron Throne must remove the affected node from the network.

If the situation arises that the owner of the Iron Throne does not want to relinquish his status after an Iron Throne vote, the network is forked. 


## Incentives
Network membership brings the following advantages:

* to use the powerful network infrastructure
* a close and decentralised exchange with other organisations
* Members are involved in the decision-making process
