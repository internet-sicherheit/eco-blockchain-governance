# Sovin Business and Technical Policies

## Business Policies

Approved members in the network are entitled to run a Validator Node each.

Candidate members need to fulfill legal requirements (must be an organisation, enterprise and fulfill formal prerequisites, etc.) in order to be approved to join the network.

A member needs to prove at least once per year that they continue to fulfill the legal requirements.

A member is suspended if:

* they are do not comply with the Network Governance
* their Validator Nodes did not achive the uptime threshold (e.g. 98% within 30 days)
* they did not take the necessary measures after a security incident occurred

The Network Governing Body can reactivate a suspended member.

When a member does not take any measure towards becoming active again, the Network Governing Body will terminate it.

## Technical Policies

A node must have one Network Interface Card (NIC) dedicated for consensus and another NIC for processing external requests. A NIC must provide a stable, static and worldwide reachable IP address.

A node must run an operating system dedicated to Validator purposes. Software other than for Validator purposes should not be running. The specific software is approved by the Technical Governance Body.

The member keys are to be stored on a different machine than the one running the Validator Node, called CLI (Command Line Interface). The Validator Node uses the keys to connect to the network. The security requirements are higher than the ones for the Validator Node.

The member need to have two points of contact for SMS alerting.

The members should make sure that the node has at least 99.9% uptime (=9 hours per year).

The member should coordinate node downtime with other members.

The network selects the active Validor Nodes that participate in the consensus using the Node Selection Algorithm. The Node Selection Algorithm selects the nodes that are less likely to fail and cause a downtime in the network.

## Sources

1. Sovrin Governance Framework, https://sovrin.org/library/sovrin-governance-framework/
2. Sovrin Steward Business Policies, https://sovrin.org/wp-content/uploads/Sovrin-Steward-Business-Policies-V2.pdf
3. Sovrin Technical and Organizational Policies, https://sovrin.org/wp-content/uploads/Steward-Technical-and-Organizational-Policies-V2.pdf
4. Sovrin Node Selection Algorithm, https://github.com/sovrin-foundation/sovrin-sip/blob/master/text/5001-node-selection-algorithm/README.md
