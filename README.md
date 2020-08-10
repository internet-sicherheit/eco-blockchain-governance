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

The general process for shaping the eBGF follows the Request for Comments ([RFC](https://www.rfc-editor.org/)) Internet publication and specification philosophy.

**We can therefore define the eBGF as the set of all eBGF RFCs.**

### Do you need an RFC?

Use an RFC to advocate substantial changes to the eBGF, 
where
those changes need to be understood by organisations implementing a governance according to eBGF and entities verfiying the validity of implementations.

### Preparation

Before writing an RFC, consider exploring the idea with the community.
TBD: Communication channels

### How to propose an RFC

  - Fork [the RFC repo](https://github.com/internet-sicherheit/eco-blockchain-governance/).
  - Pick a descriptive folder name for your RFC. Don't pick a number yet.
  - Decide which parent folder is appropriate for your RFC.
    This means aligning it with a specific working group.
  - Create the folder and copy `0000-template.md` to `<parent>/<your folder name>/README.md`.
  - Fill in the RFC. [Use MUST and SHOULD per standard conventions](https://tools.ietf.org/html/rfc2119). 
    Put care into the details: 
    RFCs that do not present convincing motivation, demonstrate an understanding of the impact of the design, or are disingenuous about the drawbacks or alternatives tend to be poorly received. 
    You can add supporting artifacts, such as diagrams and sample data, in the RFC's folder.
  - Consider how the RFC should be [tagged](/tags.md).
  - Assign a number to your RFC. Getting the number is currently a manual process which involves inspecting open and closed PRs against
    this repo to figure out what the next PR number will be (hopefully this will be changed in the future). 
    Rename your folder from `<your folder name>` to `<your 4-digit number>-<your folder name>`. 
    At the top of your README.md, modify the title so it is in the form: `<your 4-digitnumber>: Friendly Version of Your Title`. 
    We decide to use the 4-digitnumber format, to allow for easier lexical sorting.
    Commit your changes.
  - Submit a pull request.


The RFC Maintainers will check to see if the process has been followed, and request
any process changes before merging the PR.

When the PR is merged, your RFC is now formally in the `APPROVED` state.

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