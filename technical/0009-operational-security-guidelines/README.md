# 0009: Operational security guidelines
- Authors: [David Maas](david_maas@hotmail.de), [Kevin Wittek](wittek@internet-sicherheit.de), [Chinmay Khandekar](khandekar@internet-sicherheit.de) 
- Status: PROPOSED
- Since: 2020-10-21 
- Status Note: Initial Proposal  
- Start Date: 2020-10-21 
- Tags: 

## Summary
Provides the operational security guidelines

## Motivation
Operational security guidelines are required to operate a secure Blockchain infrastructure. 
Only in this way, a certain level of security and trust can be guaranteed.

## Specification
The following specifications should be implemented:
* Secure organizational structure 
* Continuous safe operation
* Regulate security for administrative staff
* Ongoing operation and integrity of your employees
* Physical security requirements
* Security requirements for outsourcing to a third-party provider
* Compliance directive for the operator?
* Authentication and authorization of the stewards and nodes in the network
* Certified that the nodes running in a secure environment
* Separation of public and internal systems regulated
* Possibilities of remote maintenance
* Realization of access control
* Update intervals of nodes and internal systems
* Regulation of access control over the network
* Authorization of the nodes in the network
 * Ensuring the ongoing integrity of the system and software


## Examples & Best Practices
We can look at the Sovrin Steward Technical and Orgnaizatoinal Policies as an example implementation:

> General Security Policies
1. A Steward MUST maintain and follow IT security policies and practices that are integral
to maintain protection of all services provided in association with the Sovrin Steward
Agreement (“Steward Services”). These policies MUST be mandatory for all employees
of the Steward involved with providing the Steward Services. The Steward shall
designate its CIO or another officer to provide executive oversight for such policies,
including formal governance and revision management, employee education, and
compliance enforcement.
2. A Steward MUST review its IT security policies at least annually and amend such
policies as the Steward deems reasonable to maintain protection of its Steward
Services.
3. Because Node administrators are a potential threat vector, a Steward MUST maintain
and follow its standard mandatory employment verification requirements for all new hires
involved with providing its Steward Services and will extend such requirements to
wholly-owned subsidiaries involved with providing its Steward Services. In accordance
with the Steward's internal process and procedures, these requirements MUST be
periodically reviewed and include, but may not be limited to, criminal background checks,
proof of identity validation, and additional checks as deemed necessary by the Steward.
Each Steward company is responsible for implementing these requirements in its hiring
process as applicable and permitted under local law.
4. Employees of a Steward involved with providing its Steward Services MUST complete
security and privacy education annually and certify each year that they will comply with
the Steward's ethical business conduct, confidentiality, security, privacy, and data
protection policies. Additional policy and process training MUST be provided to persons
granted administrative access to components that are specific to their role within the
Steward's operation and support of its Steward Services.
5. If a Steward hosts its Node in its own data center, the Steward’s security policies MUST
also adequately address physical security and entry control according to industry best
practices.
6. If the Steward hosts its Node using a third-party Hosting Provider, the Steward MUST
ensure that the security, privacy, and data protection policies of the Hosting Provider
meet the requirements in this document.
7. A Steward MUST make available to the Sovrin Foundation upon request evidence of
stated compliance with these policies and any relevant accreditations held by the
Steward, including certificates, attestations, or reports resulting from accredited
third-party audits, such as ISO 27001, SSAE SOC 2, or other industry standards.

>Node Security Policies
A Steward:
1. MUST maintain Steward keys on a separate machine from the machine that runs their
node. This machine, called the “CLI (Command Line Interface) system”, uses Steward
keys to authorize the Node to participate in the pool, and is thus the basis for trust for the
node and the Steward’s identity on the network. The CLI system is not required to have
high-end hardware, but in terms of IT best practices for security, it must meet or exceed
the standards for the Node (see following items).
2. MUST provide certification that their Node runs in a locked datacenter with appropriate
levels of security, including the specifications that they target (e.g., SSAE 16 type II
compliance; other standards may also be acceptable).
3. MUST assert that their Node is isolated from internal systems of a Steward (because the
Validator Node is publicly visible and thus an inappropriate candidate for access to
privileged internal networks).
4. MUST assert that their Node, and its underlying systems, uses state-of-the-art
authentication for remote access (at least SSH with key plus password plus source IP
firewall rule, and two-factor authentication wherever possible).
5. MUST NOT allow access (remote or local) to the Node or CLI systems by anyone other
than assigned admins.
6. MUST apply the latest security patches within one (1) week or less (24 hours or less is
recommended).
7. MUST attest that the Node runs on a server protected by a firewall that, at minimum:
* Disallows public ingress except on ports used by the Node software (different
machines may choose to expose ledger features on different ports, so no
standard port setup is required).
* Optionally enables SSH, Remote Desktop, and similar remote access tools but
constrains ingress for these tools in some way that excludes the public but allows
access for admins.
* Locks down egress ports to limit the ability to jump from Node to some other
location.
8. MUST run the Steward security check tool as requested, and MUST receive TGB
approval of the results before the Node is authorized to participate in consensus.
9. MUST run the Steward security check tool from time to time as requested by the TGB
and provide the test results report to the TGB within three (3) business days.

## Drawbacks
Too high safety requirements could lead to less network members.

## Prior art
The [Sovrin Governance Framework](https://sovrin.org/library/sovrin-governance-framework/) defines security guidelines to a certain degree as part of the [Steward Technical and Orgnaizatoinal Policies](https://sovrin.org/wp-content/uploads/Steward-Technical-and-Organizational-Policies-V2.pdf).

## Unresolved questions
Uniform certified regulations for Blockchain operators
