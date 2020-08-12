# 0001: RFC Process
- Authors: [Andrei Ionita](andrei.ionita@fit.fraunhofer.de), [Kevin Wittek](wittek@internet-sicherheit.de)
- Status: [PROPOSED](/README.md#proposed)
- Since: 2020-08-12
- Status Note: initial version  
- Supersedes:
- Start Date: 2020-08-12
- Tags: rfc, process, ebgf

## Summary

The RFC (request for comments) process is intended to provide a guideline for new features and improvements that enter the eco Blockchain Governance Framework (eBGF), so that all stakeholders and contributors are aligned with the state and evolution of the framework. 

## Motivation

The eco Blockchain Governance Framework (eBGF) serves as an abstract collection of questions and problems that need to be adressed, in order to operate a professional, production-grade, blockchain network. Hence a concrete blockchain governance which defines answers to (all) the points outlined by the eBGF can be considered a eBGF compliant blockchain governance implementation.

## Process

The eBGF is specified in the form of interconnected Markdown documents (use relative links).
Please use [Semantic Line Breaks](https://sembr.org/) for writing the Markdown documents.

If you want propose changes or new content to the framework, please either initaite a discussion in a GitHub issue or directly in a PR.

The general process for shaping the eBGF follows the Request for Comments ([RFC](https://www.rfc-editor.org/)) Internet publication and specification philosophy.

**We can therefore define the eBGF as the set of all eBGF RFCs.**

### Do you need an RFC?

Use an RFC to advocate substantial changes to the eBGF, where those changes need to be understood by organisations implementing a governance according to eBGF and entities verfiying the validity of implementations.

Before writing an RFC, consider exploring the idea with the community by opening an Issue in GitHub and stating the topic of the RFC and the reason for adding it.

### How to propose an RFC

  - Fork [the RFC repo](https://github.com/internet-sicherheit/eco-blockchain-governance/) or create a dedicated branch. Name the branch after the RFC (read below).
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

## Alternatives

Proposing RFC informally using the communication channels (Slack, Email) is in principle still possible (although discouraged). The newly proposed RFC process is designed to improve over the informal process in the following ways:

 - Discourage unactionable or vague RFCs
 - Ensure that all serious RFCs are considered equally
 - Give confidence to all contributors that they understand why new features are being merged

As an alternative, we could adopt an even stricter RFC process than the one proposed here. If desired, we should likely look to Python's [PEP]  process for inspiration.

## Unresolved questions

1. Does this RFC strike a favorable balance between formality and agility?
2. Does this RFC successfully address the aforementioned issues with the current informal RFC process?
3. Should we retain rejected RFCs in the archive?

[PEP]: http://legacy.python.org/dev/peps/pep-0001/