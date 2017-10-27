---
title: Family Member History
keywords: design, build,
tags: [design]
sidebar: foundations_sidebar
permalink: build_familymemberhistorys.html
summary: "Constructing a family member history"
---

{% include important.html content="The resources referenced in this section are the FHIR base resources which will be constrained by the profiles used by Outpatient letter, the profiles should be referred to for the actually allowable structure and content." %}

## Overview ##
This section details the design approach using FHIR resources to support the AoMRC heading model which use the FamilyMemberHistory resource. 


## Resources Used for Profile Design ##

The FHIR FamilyMemberHistory resource is profiled to create the family member history as follows:

- **[ITK-FamilyMemberHistory-1](https://fhir.nhs.uk/STU3/StructureDefinition/ITK-FamilyMemberHistory-1)** - A NHS Digital Profile for family member history. 

The record of relevant illnesses in family relations as volunteered by the patient or their carer or representative. Coded (SNOMED CT) using Family history simple reference set 999000771000000106 (foundation metadata concept). 

**Family Member History Example**

<script src="https://gist.github.com/IOPS-DEV/be1bafed8b26673bddf922b873d3975a.js"></script>




