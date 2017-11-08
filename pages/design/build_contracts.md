---
title: Contract
keywords: design, build,
tags: [design]
sidebar: foundations_sidebar
permalink: build_contracts.html
summary: "Constructing a contract"
---

{% include important.html content="The resources referenced in this section are the FHIR base resources which will be constrained by the profiles used by Outpatient letter, the profiles should be referred to for the actually allowable structure and content." %}

## Overview ##
This section details the design approach using FHIR resources to support the AoMRC heading model which use the Contract resource. The Contract resource is used for legal contracts such as Power of Attorney, Advance Statements, Advance decision to refuse treatment etc. The Contract resource may reference anything using the topic element to give the context of contract, this is constrained to an observation in the ITK profiles. The Observation profile is then further constrained to give the context applicable to the specific contract. The contract resource may contain a attachment which holds a copy of the actual document. 

## Basic Structure of Contract Profiles ##

<img src="images/build/contract_basic_structure.png" style="width:80%;max-width: 80%;">

## Resources Used for Profile Design ##
The FHIR Contract resource is profiled to create the following contract profiles:

- **[ITK-LPoA-Contract-1](https://fhir.nhs.uk/STU3/StructureDefinition/ITK-LPoA-Contract-1)** - A NHS Digital Profile for Lasting Power of Attorney.
- **[ITK-ADRT-Contract-1](https://fhir.nhs.uk/STU3/StructureDefinition/ITK-ADRT-Contract-1)** -  A NHS Digital Profile for Advanced Decision to Refuse Treatment.
- **[ITK-AdvanceStatement-Contract-1](https://fhir.nhs.uk/STU3/StructureDefinition/ITK-AdvanceStatement-Contract-1)** - A NHS Digital Profile for Advanced Statement.

The FHIR Observation resource is profiled to create the following Observation profiles:

- **[CareConnect-ITK-LPoA-Observation-1](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-ITK-LPoA-Observation-1)** - A CareConnect derived NHS Digital Profile for Lasting Power of Attorney observations.
- **[CareConnect-ITK-ADRT-Observation-1](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-ITK-ADRT-Observation-1)** -  A CareConnect derived NHS Digital Profile for Advanced Decision to Refuse Treatment observations.
- **[CareConnect-ITK-AdvanceStatement-Observation-1](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-ITK-AdvanceStatement-Observation-1)** - A CareConnect derived NHS Digital Profile for Advanced Statement.


## Last Power of Attorney Contract Example ##

<script src="https://gist.github.com/IOPS-DEV/2eba3200cfa916e3e1f17a726d9eba94.js"></script>

## Last Power of Attorney Contract and Observation Example ##

<script src="https://gist.github.com/IOPS-DEV/32f908fcbef2350535948a8c31eb3f7f.js"></script>

## Advanced Decision to Refuse Treatment Example ##

<script src="https://gist.github.com/IOPS-DEV/f18fd1c06ee1a6cbbb3706480bb2550f.js"></script>

## Advanced Statement Example ##

<script src="https://gist.github.com/IOPS-DEV/03933f4582a47ccb9903b3cc0a5e3b00.js"></script>
