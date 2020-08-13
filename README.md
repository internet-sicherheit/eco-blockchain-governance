# eco Blockchain Governance Framework - Request for Comments (eBGF-rfcs)

## Motivation and Mission Statement

The eco Blockchain Governance Framework (eBGF) serves as an abstract collection of questions and problems that need to be adressed, in order to operate a professional, production-grade, blockchain network. 
Hence a concrete blockchain governance which defines answers to (all) the points outlined by the eBGF can be considered a eBGF compliant blockchain governance implementation.

## Working Groups

In the initial step, the eBGF is structured along 4 seperate working groups(technical, legal, economy & incentives, [network governance](governance)) to handle these partial aspect of governance. 
Those should align their work with regards to the [Trust over IP](https://trustoverip.org/) Layer 1 (Utility Layer), but be open for other application contexts.
In order to keep an initial focus, the applicability of the eBGF on the blockchain technologies Ethereum and Hyperledger Indy needs to be considered.

```ascii
+----------------------------------------------------------------------------+
|                                    eBGF                                    |
|                                                                            |
|                                                                            |
|                               WORKING GROUPS                               |
| +-------------+ +--------+ +----------------------+ +--------------------+ |
| |  Technical  | |  Legal | | Economy & Incentives | | Network Governance | |
| +-------------+ +--------+ +----------------------+ +--------------------+ |
| +------------------------------------------------------------------------+ |
| |                      Trust over IP Layer1 (Utility)                    | |
| +------------------------------------------------------------------------+ |
+----------------------------------------------------------------------------+
```

### Technical

Contains guidelines and implementation recommendation, as well as best practices for aspects such as technical monitoring, hardware and software requirements, update policies, backup, disaster recovery etc. .

### Legal

Legal should describe rights, obligation and liabilities of network operators, especially according to GDPR.


### Economy & Incentives

Off-chain and on-chain economical models.
Besides obvious monetary/economical incentives, this could incentives aligned along ethcis, altruistic motives or marketing and social-networking effects.

### Network Governance

Network Governance should describe governance processes for off- and on-boarding of members into the network, proposing and executing changes to the networks' governance (which would be a concrete implementation based on the abstract eBGF), etc..


## Contribution

The eBGF is specified in the form of interconnected Markdown documents (use relative links). 
Please use [Semantic Line Breaks](https://sembr.org/) for writing the Markdown documents.

If you want propose changes or new content to the framework, please either initaite a discussion in a GitHub issue or directly in a PR.

**Please follow the guidelines in the [meta RFC](/0001-rfc-process/README.md) to initiate a PR.**

## About

#### License

This repository is licensed under an [Apache 2 License](LICENSE), in order to comply with our usage of [Aries RFCs](https://github.com/hyperledger/aries-rfcs) content.

This means that any contributions you make must be licensed in an Apache-2-compatible way,
and must be free from patent encumbrances or additional terms and conditions.
By raising a PR, you certify that this is the case for your contribution.

#### Acknowledgement

The structure and a lot of the initial language of this repository was borrowed from [Aries RFCs](https://github.com/hyperledger/aries-rfcs), which borrowed it from [Indy HIPEs](
https://github.com/hyperledger/indy-hipe), which itself borrowed it from [Rust RFC](https://github.com/rust-lang/rfcs).
There is a considerable chance that the process of ToIP will follow a same process.
