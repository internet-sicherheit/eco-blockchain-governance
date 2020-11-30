# 0047: GDPR in the context of blockchain and SSI
- Authors: [Anna Katharina Pfeiffer](a.pfeiffer@esatus.com), [Sarah Olfert](s.olfert@esatus.com)
- Status: [PROPOSED](/README.md#proposed)
- Since: 2020-10-20
- Status Note: NA
- Supersedes: NA
- Start Date: 2020-09-18 
- Tags: GDPR, SSI, blockchain, identity network

## Summary

This guide outlines what aspects of the GDPR need be considered in the context of blockchain and SSI. The main focuses are: 
- Art. 5(1) GPDR: "Basic rules" for the legally compliance of processing personal data
- Art. 25 GDPR: Privacy by Design and Default 
- Art. 32 and 35 GDPR: Technical and organizational measures according and data protection impact assessment 

## Motivation
Due to the European Genereal Data Protection Regulation (GPDR) the handling of personal data is an important issue when it comes to setting up an IT solution. This is also true for blockchain and especially for identity networks focusing on Self-Sovereign Identity (SSI). Many identity networks are in establishment and GDPR compliance is one of the key success factors to gain acceptance in the community. This guide outlines what aspects of the GDPR need to be considered in this context.

## Specification

### Personal Data Processing Principles and Permissions 

The European General Data Protection Regulation focuses on six so-called principles for the legally compliant processing of personal data. The six principles pursuant to Art. 5(1) GDPR represent the "basic rules" for the legally compliant processing of personal data and must therefore be complied with accordingly.

The following section examines how and by which appropriate measures the respective principle in Art. 5(1) GDPR is fulfilled. 

#### Lawfulness of data processing according to Art. 5(1)a) GDPR

The GDPR defines the principles of transparency, lawfulness and good faith in Art. 5(1)a) GDPR. The GDPR stipulates that processing must be lawful, in good faith and in a manner that is comprehensible to the person concerned. In terms of general data protection regulation, lawfulness means that the processing of personal data may only be carried out on the basis of a valid legal basis. Personal data can therefore only be processed if one of the six following legal bases is applicable. Art. 6(1) GDPR defines the following legal bases: Consent for specific purposes; fulfillment of obligations arising from a contractual relationship; fulfillment of legal obligations; safeguarding vital interests; performance of a task which is in the public interest or is carried out in the exercise of official authority; safeguarding legitimate interests.

In the context of SSI, this means that the lawfulness of the data processing is fulfilled by the authorization from Art. 6(1)a) GDPR - consent for specific purposes.

By using credentials and a corresponding wallet, users can independently manage their identity and its attributes and control which data they pass on to which institution. This is possible because with each credential query, the user sees what data is requested from him. The user then decides independently whether or not to release or transmit the corresponding information. A declaration of consent is therefore given before any personal data is passed on. In addition, the user has the opportunity to issue permanent declarations of consent, which he can revoke independently.

Transparency in the sense of general data protection regulation means that all information and notifications concerning the processing of personal data must be written in clear and uniform language. As a rule, compliance with this principle is achieved by creating and providing the so-called information obligations in accordance with Art. 13 GDPR. The information duties inform the data subject about

- Contact details of the data controller including contact details of the data protection officer

- Purposes and legal basis of the processing

- Recipients or categories of recipients

- Transfer of personal data to a third country

- Duration of storage

- Rights of data subjects

This means that as soon as personal data is processed, the corresponding information (according to Art. 13 GDPR) is made available.

#### Purpose limitation according to Art. 5(1)b) GDPR

Purpose limitation in the sense of general data protection regulation means that processing is only permitted for specified, clear and legitimate purposes. For this purpose, as already mentioned the GDPR defines six principles. Personal data may therefore only be processed if it is based on one of the six legal bases mentioned above. 

#### Data minimization and storage limitation according to Art. 5(1)c) and e) GDPR

Another important factor in the processing of personal data is data minimization and memory limitation. It is important to ensure that the processing of personal data is limited to a necessary extent and that only the data that is really necessary is processed. 

In the context of the identity network, this means that when processing personal data, the sending and storage of data must be reduced to a minimum. By using the identity network, only the user has the sovereignty of his data. The user decides independently which personal data he wants to disclose to which recipient. In addition, it is possible to trace at any time when which personal data was requested and released. A period of validity can be specified when issuing credentials. As soon as this validity period is exceeded, the credential can no longer be used for authentication or authorization. The personal data contained in the credentials issuing system must be deleted in accordance with the respective storage periods. This deletion of this data is the responsibility of the responsible party.

#### Accuracy of the data according to Art. 5(1)d) GDPR

In doing so, all reasonable steps shall be taken to ensure that personal data which are inaccurate in relation to the purposes for which they are processed are erased or rectified without delay.

#### Integrity and confidentiality according to Art. 5(1)f) GDPR

Appropriate technical and organizational measures must be taken to protect the data from unauthorized or unlawful processing, accidental loss, destruction or damage. 

#### Accountability according to Art. 5(2) GDPR

Since the GDPR came into force, the person responsible is responsible for compliance with Art. 5(1) GDPR and must be able to prove that this has been complied with. In order to comply with this obligation, appropriate data protection documentation must be prepared. This includes: a list of processing activities in accordance with Art. 30 GDPR, documentation of the technical and organizational measures (TOMs) taken in accordance with Art. 32 GDPR as well as the information obligations in accordance with Art. 13 GDPR. In addition, appropriate contracts must be concluded between the person responsible and the processor. As soon as processing is carried out on behalf of a controller, the controller may only work with processors who offer sufficient guarantees that appropriate technical and organizational measures are implemented in such a way that the processing is carried out in accordance with the requirements of the GDPR and guarantees the protection of the rights of the data subject. In order to be able to prove this compliance as the person responsible, a so-called data processing agreement must be concluded between the parties involved.

### Privacy by Design and Default

Already in the early phase of product development and design, data protection should be a mandatory part of the development process and a comprehensive examination of the processed data, the purposes associated with it and, in particular, the technical and organizational measures should be carried out in order to ensure data protection in the sense of the Regulation. Art. 25 GDPR formulates, among other things, the principle of Privacy by Design. This means that data protection should be incorporated into product design as early as the development and implementation stages.

In order to meet the requirements of Art. 25 GDPR, it is necessary to take appropriate measures at an early stage. It is helpful here to take Art. 25 GDPR into account when managing data security within the company. In addition, an appropriate risk analysis and evaluation of the risks and the resulting consequences should be carried out.

### Technical and organizational measures according to Art. 32 GDPR

On the basis of the records of the processing activities (Art. 30 GDPR), the data protection officer weighs up what risks (could) arise for the rights and freedoms of the data subject as a result of the data processing. If necessary, the data controller will carry out a data protection impact assessment (Art. 35 GDPR) following this consideration.

On the basis of this risk assessment, the data controller decides which TOMs are to be implemented in order to keep the risk to the data subject as low as possible. Two conclusions for TOMs follow from this risk-based approach: 

1. different TOMs are possible, if not necessary, for different processing operations 

2. the data controller must regularly and systematically adapt the TOM to the state of the art. This is particularly necessary for processing operations that have been legally required for decades. 

TOM must not be understood as something considered once only, but as an ongoing obligation that is in a continuous process. Those responsible for data protection meet this ongoing challenge by keeping themselves constantly informed about the state of the art and by following developments in the field of data protection. 

In the German legal area, the following features from Section 64 of the Federal Data Protection Act (Bundesdatenschutzgesetz) can be used for the documentation of TOMs, due to their compatibility.

- Equipment access control according to Section 64(3)no.1 Federal Data Protection Act: It must be ensured that the persons authorized to use an automated processing system have access only to the personal data covered by their access authorization.

- Data media control according to Section 64(3)no.2 Federal Data Protection Act: It must be ensured that personal data cannot be read, copied, changed or deleted by unauthorized persons. 

- Storage control according to Section 64(3)no.3 Federal Data Protection Act: The prevention of the unauthorized entry of personal data as well as the unauthorized inspection, modification and deletion of stored personal data must be ensured by appropriate measures.

- User control according to Section 64(3)no.4 Federal Data Protection Act: It must be ensured that the persons authorized to use an automated processing system have access exclusively to the personal data covered by their access authorization. Furthermore, it must be ensured that personal data cannot be read, copied, changed or deleted by unauthorized persons during processing, use and after storage (Section 64(3) No.2,3,5 Federal Data Protection Act).

- Data access control according to Section 64(3)no.5 Federal Data Protection Act: It must be ensured that it can be subsequently checked and established which personal data have been entered or modified in automated processing systems, at what time and by whom (Section 64(3)no.3 Federal Data Protection Act).

- Communication control according to Section 64(3)no.6 Federal Data Protection Act: It is necessary to prevent the use of automated processing systems by third parties with the aid of data transmission equipment. It must be ensured that it is possible to check and establish at which points personal data have been or can be transmitted or made available with the aid of data transmission equipment (Section 64(4),(6) Federal Data Protection Act).

- Input control according to Section 64(3)no.7 Federal Data Protection Act: It must be ensured that it can be subsequently checked and established which personal data have been entered or modified in automated processing systems, at what time and by whom.

- Transport control according to Section 64(3)no.8 Federal Data Protection Act: It must be ensured that the confidentiality and integrity of the data is protected during the transmission of personal data and the transport of data carriers. 

- Recovery according to Section 64(3)no.9 Federal Data Protection Act: It must be ensured that systems in use can be restored in the event of a fault.

- Reliability according to Section 64(3)no.10 Federal Data Protection Act: It must be ensured that all functions of the system are available and that occurring malfunctions are reported.

- Integrity according to Section 64(3)no.11 Federal Data Protection Act: It must be ensured that stored personal data cannot be damaged by malfunctioning of the system and that new or modified programs do not lead to malfunctions or security gaps in the systems.

- Processing control according to Section 64(3)no.12 Federal Data Protection Act: It must be ensured that personal data processed by order can only be processed according to the instructions of the client.

- Availability control according to Section 64(3)no.13 Federal Data Protection Act: It must be ensured that personal data is protected against destruction or loss by appropriate data security measures and that systems used can be restored in the event of a fault.

- Separability according to Section 64(3)no.14 Federal Data Protection Act: It must be ensured that personal data collected for different purposes can be processed separately.

### Data protection impact assessment

A Data Protection Impact Assessment (DPIA) is a document that describes and assesses the processing of personal data in a processing operation subject to an impact assessment. In particular, the risks to the rights and freedoms of natural persons arising from the processing operation must be assessed and adequately mitigated by appropriate countermeasures. In addition, the person responsible for the respective processing operation can thus prove that he has selected the appropriate measures so that processing in compliance with the regulations is possible. A DPIA refers here to the processed data, the hardware and software used and the processes used in a specific processing operation. 

It is possible to carry out a single DPIA for several similar processing operations with similarly high risks - keyword cumulative DPIA - see Art. 35(1)1 sentence 2 GDPR.

The execution of a DPIA is in principle (only) mandatory if the processing activity is a (suspected) high-risk processing. According to Art. 35(1) Sentence 1 GDPR, the person responsible must carry out a DPIA in advance for processing operations which are likely to present a high risk to the rights and freedoms of natural persons. The high risk can result from the type, scope, circumstances and purposes of the processing, especially if new technologies are used.

#### Pre-analysis risk

Recitals 75 and 76 of the GDPR define the risks to the rights and freedoms of data subjects. 

Recital 75: A risk within the meaning of the GDPR is the existence of the possibility of an event occurring which in itself constitutes damage (including unjustified impairment of the rights and freedoms of natural persons) or which may result in further damage to one or more natural persons. It has two dimensions: First, the severity of the damage and second, the probability that the event and the consequential damages will occur.

Recital 76: "The likelihood and seriousness of the risks to the rights and freedoms of the data subject should be determined by reference to the nature, extent, circumstances and purposes of the processing. The risk should be assessed on the basis of an objective evaluation determining whether the data processing involves a risk or a high risk.

#### Examination of the characteristics from Art. 35(3) GDPR

A data protection impact assessment referred to in paragraph 1 shall in particular be required in the case of:

- a systematic and extensive evaluation of personal aspects relating to natural persons which is based on automated processing, including profiling, and on which decisions are based that produce legal effects concerning the natural person or similarly significantly affect the natural person;

- processing on a large scale of special categories of data referred to in Art. 9(1), or of personal data relating to criminal convictions and offences referred to in Art. 10; or

- a systematic monitoring of a publicly accessible area on a large scale.

In addition to Art. 35(3) GDPR, the competent supervisory authority shall draw up a list of processing operations for which a data protection impact assessment must be carried out (so-called must-list or blacklist) in accordance with Art. 35(4) GDPR, due to a likely high risk to the rights and freedoms of natural persons.The supervisory authority shall draw up and publish a list of processing operations for which a data protection impact assessment must be carried out in accordance with paragraph 1. Furthermore, the supervisory authority may draw up and publish a list of the types of processing operations for which a data protection impact assessment is not required. 

#### Review of the black/white lists of the supervisory authorities according to Art. 35(4) GDPR

In assessing whether a processing operation is likely to present a high risk, the following nine criteria must be taken into account.

1. evaluation and classification: The processing activity shall include an assessment or classification of data subjects. This includes, for example, the drawing up of profiles and forecasts, in particular on the basis of aspects relating to the performance of work, the economic situation, health, personal preferences or interests, reliability or behaviour, whereabouts or change of location of the person concerned.

2. automated decision making with legal effect or similar interpretative effect:On the one hand, the exclusively automated decision making is covered, and on the other hand a decision making for which automated processing makes a significant contribution. In both cases, the decisions must have a legal effect on natural persons or affect them in a similarly significant way. These conditions are met, for example, if the automated processing leads to the exclusion or disadvantage of natural persons.

3. systematic monitoring: The purpose of the processing operation is the observation, monitoring or control of data subjects and relies, for example, on data collected by networked sensors and cameras or on systematic surveillance of publicly accessible areas (Art. 35(3)c GDPR).

4. confidential or highly personal data: During processing, confidential or highly personal information is processed. The following categories in particular must be taken into account:

- Special categories of personal data according to Art. 9(1) or Art. 10 GDPR,

- Social data according to Art. 35 of the First Book of the Social Code - General Part -, so far not already covered by Art. 9(1) GDPR, and

- Financial data that allows comprehensive information about the financial circumstances of the person concerned, or that can be misused for payment fraud.

5. large-scale data processing: In assessing whether data processing is large-scale, the following factors (cumulative) in particular must be taken into account:

- The number of data subjects: consideration of either the actual number of data subjects (absolute consideration) or the proportion of the population concerned (relative consideration)

- Data volume: processed data volume or bandwidth of the different processed data elements

- Duration: Duration or permanence of data processing

- Geographic scope: Geographic extent of data processing

6. matching or merging records: The processing operation involves the direct integration and/or comparison of data sets from two or more processing operations carried out for different purposes and/or by different controllers in a way that goes beyond the reasonable expectations of the data subjects.

7. data of data subjects in need of protection (see recital 75 GDPR): During processing, data relating to vulnerable data subjects are mainly processed. This includes in particular the following groups of persons:

- Children,

- Other persons in need of protection (e.g. persons who are legally incapable and/or in psychiatric care; severely disabled persons; asylum seekers)

- Employees in situations of superiority and subordination to their employer/supervisor

8. Innovative use or application of new technological or organizational solutions: During the processing procedure, technologies that are to be classified as new according to the current state of the art or new organizational solutions are used. The potentially high risk to rights and freedoms can arise here in particular from the novel form of data collection or use and from the fact that the effects on the data subjects and society are difficult to assess.

9. data subjects are prevented from exercising a right or using a service or performing a contract: The processing operation itself prevents the data subject from exercising a right, using a service or performing a contract.

If two of these criteria are met, in most cases a data protection impact assessment must be carried out. The more criteria are met, the more likely it is that a privacy impact assessment will be carried out. However, it is also possible that there is a high risk if only one criterion is met.

#### Conclusion Necessity of data protection impact assessment before productive use

If a DPIA shows that despite the selected and implemented TOMs for risk mitigation, a high risk for the persons concerned still exists, the competent supervisory authority must be consulted pursuant to Art. 36 GDPR. A decision must then be made, taking into account the recommendations of the supervisory authority, as to whether the processing operations can be carried out in view of the remaining residual risks and whether additional TOMs need to be adopted. It should be noted that the supervisory authority may issue a warning, instruction or prohibition.

### Conclusion 
In order to be able to give a comprehensive assessment of the conformity with the GDPR, all the above-mentioned areas must be checked and documented. By this procedure, areas in which a need for action exists are pointed out and can be improved accordingly by the responsible party.

The points listed represent an aid to the GDPR. From the German point of view, it was shown which requirements for the data protection compliant processing of personal data must be considered

- Data privacy importance
- acceptance 

## Examples & Best Practices
There are not many publications from existing identity providers which address the topic blockchain and GDPR. There is a published [report](https://sovrin.org/gdpr-position-paper/) from the [Sovrin Foundation](https://sovrin.org/) where they analyze wheter and how the GDPR applies to them. But many identity networks such like [IDunion](https://idunion.org/), [Bedrock](https://bedrock-consortium.github.io/bbu-gf/gf_info/business_model_concepts/), [uPort](https://www.uport.me/) or [Indicio](https://indicio.tech/) are still in the establishment phase. Therefore statements how they address GDPR requirements are not published yet. 

Other important publications which cover the topic a bit would be:
- [Self-sovereign Identity - A position paper on blockchain enabled identity and the road ahead](https://www.bundesblock.de/wp-content/uploads/2019/01/ssi-paper.pdf) from [Blockchain Bundesverband](https://bundesblock.de/de/)
- [Decentralised Identity: What's a Stake?](https://inatba.org/wp-content/uploads/2020/11/2020-11-INATBA-Decentralised-Identity-001.pdf) from [INATBA](https://inatba.org/)
- [SSI in action](https://esatus.com/wp-content/uploads/Actionlog_BAS_SSI_in_der_praktischen_Nutzung_20201009.pdf) from [esatus AG](https://esatus.com/)

## Drawbacks
NA

## Prior art
NA

## Unresolved questions
- One advantage of blockchain which strenghtens the integrity of data is in the same time one big challenge within GDPR. If once something is written on-chain it can not be removed afterwards. This hurdens the implementation of "the right to be forgotten" (Art. 17 GDPR). One technical possibility is known under the word "tombstoning". A mark associated with a transaction indicating that the transaction may no longer be returned in response to read access requests. But tombstoning still needs to be recognized and accepted by law, because it is only a kind of blocking notice.
