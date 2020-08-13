# 0004: Suspension and Termination of members
- Authors: Andrei Ionita (andrei.ionita@fit.fraunhofer.de)
- Status: [PROPOSED](/README.md#proposed)
- Since: 2020-08-13
- Status Note: added review suggestions
- Supersedes:
- Start Date: 2020-08-12
- Tags: governance, suspension, termination, sanction, exclusion, offboarding, off-boarding

## Summary

Establishes the circumstances in which members of the network are suspended and terminated due to rule violations.  

## Motivation

In order to prevent abuse and encourage members to take responsibility in the network, the governance includes the possibility of penalties, suspension and termination of members.  

## Specification

An implementation should consider the following points. The list is by no means complete.

* not complying with the network governance terms

* member organisations that violate any legal terms or are in dispute with the network organisation

* failure to achieve a certain degree of availability over a fixed period of time 

* failure to take certain measures after experiencing a security intrusion

* inactivity for a certain period of time

* suspension prevents party to re-apply for network membership for a certain period of time

* re-applying for network membership after suspension includes providing proof that certain measures have been taken that prevent future suspension

* suspension is an intermediate step prior to termination

* a member is terminated when the network governing body takes the decision by vote 

* a suspended member that does not re-apply for membership is selected for termination

* re-applying for network membership after termination includes providing proof that certain measures have been taken that prevent future suspension and termination

* a member that has been terminated multiple times cannot apply for network membership anymore

## Examples & Best Practices

Sovrin regulates suspension in its [Steward Business Policies] as follows:

> A Steward MUST be suspended by the responsible Sovrin Governing Body under any of the following conditions:

> * The Steward no longer complies with the Steward Business Policies, Steward
Technical Policies, or any other requirements of the Sovrin Governance
Framework.

> * The Steward’s Node has failed to achieve 98% availability over a period of 30
days.

> * A security intrusion or violation has been reported and the Sovrin Technical Governance Board is not satisfied that the Steward has performed adequate
remediation.

> * The Steward fails to requalify under its annual requalification process specified [..]

> * The Steward has, in the sole judgment of the Sovrin Board of Trustees, violated
some or all of the Sovrin Governance Framework principles, taken action against
the purpose of the Sovrin Foundation, or has shown behaviour contrary to the
collective interest of the Sovrin Foundation or performed action that brought the
Sovrin Foundation or the Sovrin Network into disrepute.

> A Steward who is suspended MUST not have an active Node on any Sovrin Ledger
network until such time as Steward is able to provide reasonable assurance to the
responsible Sovrin Governing Body that:

> * The Steward is back in compliance with all requirements of the Sovrin
Governance Framework, and

> * The Steward has the ability to maintain compliance for the foreseeable future.

> At the request of a suspended Steward, the responsible Sovrin Governing Body MUST
examine the Steward’s remediation efforts and make one of the following decisions: 

> * Reactivate the Steward
> * Request further remediation by the Steward 
> * Terminate the Steward.

Furthermore, Termination is implemented as follows:

> * A Steward who has breached the terms of the Sovrin Steward Agreement MAY be
terminated by a majority vote of the responsible Sovrin Governing Body with ratification
by the Board of Trustees.

> * A Steward who has been suspended and not been reactivated within 180 days following
suspension MUST be notified of automatic termination.

> * An Organization who has been previously terminated as a Steward and who applies to
be reinstated MUST disclose the previous termination in their application and explain the
remediation steps that the Steward has taken to requalify.

Bloxberg implements suspension and termination in its [Whitepaper] as *sanction* and respectively *exclusion*:

> Sanctions (revoke membership) can be taken if a member misbehaves. The exclusion of a
Authority node in the bloxberg network has to be approved by a voting of the bloxberg consortium
members.
> Events that will trigger a sanctions voting:
> 1. A Authority node is offline for > 3 month
> 2. A Authority node spams the network
> 3. The member acts in a non-compliant manner according to the governance model
> 4. The entity is not aligned with the manifesto
> Voting for the exclusion of a bloxberg consortium member:
> 1. A voting for exclusion will be triggered if one of the above mentioned events occur
> 2. The voting is executed off-chain
> 3. The voting is executed according to the bloxberg decision algorithm
> 4. The bloxberg consortium needs a quorum of >75% to execute a valid voting, but a minimum of 7 voting organizations.
> 5. If > 75% of the valid votes are yes, the member is excluded
> 6. The Iron Throne is instructed to exclude the member from the bloxberg network
> 7. The excluded organization can reapply for a bloxberg consortium membership

## Drawbacks

Keeping members in the network may help increase the network size and popularity. Exclusion of members may also be linked to censorship and centralization. Furthermore, suspension may deter parties to rejoin the network. 

## Prior art

The [Sovrin Governance Framework](https://sovrin.org/library/sovrin-governance-framework/) has well-defined governance policies for suspension and termination in its [Steward Business Policies].

[Bloxberg](http://bloxberg.org) refers to suspension and termination as *sanction* and *exclusion* in its [Whitepaper], which applies for validator members.

## Unresolved questions

* Distinction between validator members, i.e. members that run a node, and simple members has not been made

[Steward Business Policies]: https://sovrin.org/wp-content/uploads/Sovrin-Steward-Business-Policies-V2.pdf
[Whitepaper]: https://bloxberg.org/wp-content/uploads/2020/02/bloxberg_whitepaper_1.1.pdf
