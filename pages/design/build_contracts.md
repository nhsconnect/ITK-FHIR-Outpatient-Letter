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
This section details the design approach using FHIR resources to support the AoMRC heading model which use the Contract resource. The Contract resource is used for legal contract such as Power of Attorney, Advance Statements, Advance decision to refuse treatment etc. 

## Resources Used for Profile Design ##
The FHIR resources are profiled to create contracts as follows:

- **[ITK-LPoA-Contract-1](https://fhir.nhs.uk/STU3/StructureDefinition/ITK-LPoA-Contract-1)** - A CareConnect derived NHS Digital Profile for Lasting Power of Attorney.
- **[ITK-ADRT-Contract-1](https://fhir.nhs.uk/STU3/StructureDefinition/ITK-ADRT-Contract-1)** -  A CareConnect derived NHS Digital Profile for Advanced Decision to Refuse Treatment.
- **[ITK-AdvanceStatement-Contract-1](https://fhir.nhs.uk/STU3/StructureDefinition/ITK-AdvanceStatement-Contract-1)** - A CareConnect derived NHS Digital Profile for Advanced Statement.


## Contract Examples ##

**Lasting Power of Attorney**

<script src="https://gist.github.com/IOPS-DEV/c01035964aa03df1438a6f2e87448989.js"></script>

**Advanced Decision to Refuse Treatment**

**Advanced Statement**

