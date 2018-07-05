---
title: Messaging Interactions
keywords:  messaging, interactions
tags: [fhir,messaging,interactions]
sidebar: foundations_sidebar
permalink: explore_interactions.html
summary: "ITK3 Outpatient Letter Interactions"
---




## ITK3 Outpatient Letter Interactions Overview ##
This section provides ITK3 Outpatient Letter implementers with the information required to utilise the ITK3 Outpatient Letter Interactions.

**Note 1:** When using MESH, additional MESH acknowledgements and responses will be available.  The MESH acknowledgements and responses are not defined in this specification

**Note 2:** Messages are structured in eXtensible Markup Language (XML) only.

The ITK3 Outpatient Letter is based on the [HL7 FHIR STU3 Messaging Implementation](http://hl7.org/fhir/messaging.html) and supports multiple interactions. 

---------
## DOC-ToC-Primary-Recipient-OutpatientLetter-1 Interaction ##

The sending hospital system will construct an Outpatient Letter FHIR Document and send it to the primary recipient's receiving system.

- Sender: Hospital sending system
- Receiver: Outpatient Letter Recipient system
- Message: Wire Format: TOC-OutpatientLetter-1

## DOC-ToC-Copy-Recipient-OutpatientLetter-1 Interaction ##

The sending hospital system will construct an Outpatient Letter FHIR Document and send it to the copy recipient's receiving system. 

- Sender: Hospital sending system
- Receiver: Outpatient Letter Recipient system
- Message: Wire Format: TOC-OutpatientLetter-1

## Acknowledgements Interactions ##

Dependent on system set up the following interactions may be utilised.


- <a href="https://nhsconnect.github.io/ITK3-FHIR-Messaging-Distribution/explore_interactions.html#rsp-itk-infrastructure-acknowledgement-response-1-interaction" target="_blank">RSP-ITK-Infrastructure-Acknowledgement-Response-1</a>
- <a href="https://nhsconnect.github.io/ITK3-FHIR-Messaging-Distribution/explore_interactions.html#rsp-itk-business-acknowledgement-response-1-interactions" target="_blank">RSP-ITK-Business-Acknowledgement-Response-1</a>

## Outpatient Letter ITK3 FHIR Document Interactions Diagram  ##

The diagram shows the Outpatient Letter Document Interactions: Note: The use of the ITK3 infrastructure interactions are dependent on system configuration.  


<img src="images/explore/ITK-Outpatientletter-FHIRInteractions.png" style="width:75%;max-width: 75%;">












