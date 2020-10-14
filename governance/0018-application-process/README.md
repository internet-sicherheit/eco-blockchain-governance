
# RFC 0018: Application process for new members
- Authors: Tina Marquardt (marquadt@internet-sicherheit.de) and Chinmay Khandekar (khandekar@internet-sicherheit.de) 
- Status: [PROPOSED](/0001-rfc-process/README.md)
- Since: 2020-08-12 
- Status Note: Draft
- Supersedes:
- Start Date: 2020-08-01
- Tags: governance, onboarding, member, application, process

## Summary

The RFC provides a guidelines for an possible application process to select new members to join a consortial blockchain network.
 
## Motivation

A transparent application process flow provides a clear and transparent overview to the applicant and members. 
It increases confidence that their application has been scrutinized well before a decision is made and that only elgibile and trustworthy organizations are able to join.
The process gives equal chances to all eligible applicants and creates more security within the exisiting consortia. 


## Specifications

* Workflow process for the applying organization when applying to join consortial blockchain network.
* This RFC needs to be combined with [#0003RFC](https://github.com/internet-sicherheit/eco-blockchain-governance/tree/master/governance/0003-Onboarding)
* Criteria to evaluate applicants
* Decision-making on new applicants, for more details refer to [#0020RFC](https://github.com/internet-sicherheit/eco-blockchain-governance/issues/44) for more information on decision-making in governance processes)
* Interval for internal decision or voting to decide on applicants
* Different Classes of Membership imply different rights and nodes for members
* Degree of transparency of the process e.g. publication on a website
* Is there something like an alternating comitee?

## Examples & Best Practices

Sovrin regulates applications process in its [Sovrin Business Policy V2 Policy](https://sovrin.org/wp-content/uploads/Sovrin-Steward-Business-Policies-V2.pdf) as follows:

### Application process for the organization when applying:
> * The Sovrin Foundation Steward application and selection process MUST:
>   ** Use the Core Principles of the Sovrin Governance Framework as a guide, with special attention to the Decentralization by Design principles.
>   ** Be publicly documented on the Sovrin Foundation website.
> * To apply, an Organization MUST submit a written application to the Sovrin Governing Body responsible for Steward applications as directed on the Sovrin Foundation website.
> * The Steward application process MUST follow the guidelines for Self-Certification, Certification, or Accreditation as specified by the Sovrin Trust Assurance Framework.
> * In evaluating and prioritizing Steward applications, the Sovrin Foundation MUST take into account:
>   ** Public contributions of any kind, including but not limited to open source engineering resources, efforts to drive Sovrin adoption, participation in Sovrin governance, marketing efforts, and direct financial contributions, that the prospective Steward has made in the past to the Sovrin Foundation or the Sovrin Community.
>   ** Public contributions of any kind the prospective Steward commits (in writing in its Steward application) to making to the Sovrin Foundation or the Sovrin Community.
> * Any other specific Practices and Procedures involved in the Steward application process MUST be publicly documented on the Sovrin Foundation website.

Bloxberg defines new member application workflow in its [Bloxberg Whitepaper v1.1](https://bloxberg.org/wp-content/uploads/2020/02/bloxberg_whitepaper_1.1.pdf) as follows:
> * Voting for new bloxberg consortium members. Workflow:
>   ** Applicant fills out a form on the official (bloxberg.org) website
>   ** The Iron Throne adds the applicant to the voting dApp
>   ** Once every 4 weeks members vote for 4 weeks on new applicants
>   ** The voting is executed on-chain after an off-chain discussion
>   ** The voting is executed according to the bloxberg decision algorithm, refer to [#0020 RFC](https://github.com/internet-sicherheit/eco-blockchain-governance/issues/44) for more information on decision-making in governance processes)
>   ** The bloxberg consortium needs a quorum of >50% of all voting power, to execute a valid voting, but a minimum of 3 voting organizations.
>   ** If > 50%of the valid votes are yes, the new member is accepted. If not, the new member is rejected and can reapply at a later time.
>   ** After a positive vote the Iron Throne is instructed to add the new member as a authority node to the bloxberg network.
>   ** The new member has to run one Authority node, but can have n non-Authority nodes. The Authority node must be available in the network all the time.


## Drawbacks 

* In case the decision is met by members on chain, anonymity cannot be assured (pseudonimity at best)
* Long application process may not seem contemporary for new members

## Prior art

* The [Sovrin Business Policy V2 Policy](https://sovrin.org/wp-content/uploads/Sovrin-Steward-Business-Policies-V2.pdf) and [Bloxberg Whitepaper v1.1](https://bloxberg.org/wp-content/uploads/2020/02/bloxberg_whitepaper_1.1.pdf) has been used to retrieve possible answers within this document. 

## Unresolved questions

* Best Practice for decision-making in more decentralized governance syststems 
* Are there other criteria that need to be considered for new applicants?
* How can this application process be changed?
