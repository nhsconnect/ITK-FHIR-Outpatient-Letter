---
title: Observation
keywords: design, build,
tags: [design]
sidebar: foundations_sidebar
permalink: build_observations.html
summary: "Constructing a observation"
---

{% include important.html content="The resources referenced in this section are the FHIR base resources which will be constrained by the profiles used by Outpatient letter, the profiles should be referred to for the actually allowable structure and content." %}

## Overview ##
This section details the design approach using FHIR resources to support the AoMRC heading model which use the observation resource. The observation resource is referenced from the Condition resource. There are other more specialised observation profiles which as documented in the specialised observation section.


## Resources Used for Profile Design ##
The FHIR resources are profiled to create the observation as follows:

- **[CareConnect-ITK-Observation-1](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-ITK-Observation-1 )** - A CareConnect dervived NHS Digital Profile for observation. The Observation resource is used for tracking the current and historical observations that have been made for a patient.

## Observation ##
This resource is used to record information tracking the current and historical observations that have been made for a patient.The following is a example of the elements that can be used: 

- identifier - uniquely identifies this observation (UUIDs)
- Status - 	registered,preliminary,final,amended etc
- code - identification of the observation
- performer - who made the observation
- subject - the patient
- interpretation - High,Low, Normal etc
- bodySite - the part of the body the observation was made about
- method - How it was done 


**Observation Example**

<script src="https://gist.github.com/IOPS-DEV/c01035964aa03df1438a6f2e87448989.js"></script>

## Specialised Observation Profiles ##

This section gives information about the specialised observation profiles. These are derived from the CareConnect observation profile  but are every tightly constrained for a particular ITK use case.

The current specialised profiles are:

## Accessible Information Observation ##

- **[CareConnect-ITK-AccessibleInformation-Observation-1](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-ITK-AccessibleInformation-Observation-1)**

Information volunteered by the person or their representative or carer, or known about locally.
Coded using SNOMED CT, constrained as specified in SCCI1605.
Accessible Information standard (accessible information - communications support, accessible information - requires communications professional, accessible information - requires specific contact method, accessible information - requires specific information format). Uses the following subsets:

**Personal Preferences subset**

- **[Personal Preferences](https://dd4c.hscic.gov.uk/dd4c/publishedmetadatas/intid/225)**

**Accessible information subsets**

- **[Accessible information - communication support](https://dd4c.hscic.gov.uk/dd4c/publishedmetadatas/intid/657)**
- **[Accessible Information - requires specific information format](https://dd4c.hscic.gov.uk/dd4c/publishedmetadatas/intid/660)**
- **[Accessible Information - requires communication professional](https://dd4c.hscic.gov.uk/dd4c/publishedmetadatas/intid/658)**
- **[Accessible Information - requires specific contact method](https://dd4c.hscic.gov.uk/dd4c/publishedmetadatas/intid/659)**

**Mobility subsets**

- **[Mobility findings](https://dd4c.hscic.gov.uk/dd4c/publishedmetadatas/intid/762)**
- **[Mobility Issues](https://dd4c.hscic.gov.uk/dd4c/publishedmetadatas/intid/181)**
 
**Cognition**

- **[Cognition](https://dd4c.hscic.gov.uk/dd4c/publishedmetadatas/intid/9)**

## Accessible Information Observation Example ##

<script src="https://gist.github.com/IOPS-DEV/c8f907c31495b106f871d054f419dedb.js"></script>

## Advanced Decision to Refuse Treatment Observation ##
 
- **[CareConnect-ITK-ADRT-Observation-1](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-ITK-ADRT-Observation-1)**

For more information of SNOMED CT codes (see National Information Standard (SCCI1580). Location of ADRT should be recorded as free text. Where available a copy of the ADRT may be appended to the record using the bindingAttachment element of the Contract resource. Where there has been a change in the ADRT this should be noted in the record in free text of the relevant section.

## Advanced Decision to Refuse Treatment Observation Example ##

<script src="https://gist.github.com/IOPS-DEV/bea759e103666e310d8ecf7089ced872.js"></script>

## Advance Statement Observation ##

- **[CareConnect-ITK-AdvanceStatement-Observation-1](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-ITK-AdvanceStatement-Observation-1)**	

A record of the presence of an advance statement using the following SNOMED CT concept from the National Information Standard (SCCI1580): SNOMED CT: 816281000000101. Has advance statement (Mental Capacity Act 2005). The content of the advance statement should also be included as text in the text section or attached as a document where available using bindingAttachment element of the Contract resource.

## Advance Statement Observation Example ##

<script src="https://gist.github.com/IOPS-DEV/933392fa6e35bd348c380980380db1de.js"></script>

## Cognition Observation ##
	
- **[CareConnect-ITK-Cognition-Observation-1](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-ITK-Cognition-Observation-1)**



## Lasting Power of Attorney Observation ##		
- **[CareConnect-ITK-LPoA-Observation-1](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-ITK-LPoA-Observation-1)**	

## 	Mobility-Observation ##
- **[CareConnect-ITK-Mobility-Observation-1](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-ITK-Mobility-Observation-1)**	
- 
## OccupationalHistory-Observation ##	
- **[CareConnect-ITK-OccupationalHistory-Observation-1](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-ITK-OccupationalHistory-Observation-1)**
		
 

 
