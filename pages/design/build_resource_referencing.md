---
title: Resource referencing
keywords: resource
tags: [development,fhir,profiles]
sidebar: overview_sidebar
permalink: build_resource_referencing.html
summary: "Resource referencing explained."
---

{% include custom/search.warnbanner.html %}

## Overview ##
This section details the reference between resources.

The diagrams only go to one level due to the complexity and size of the message.Below is the key to the diagrams.

<img src="images/explore/Key.png" style="width: 75%;max-width: 75%;"> 



## ITK Outpatient letter FHIR Document ##

The diagram shows the referencing between the profiles in the bundle which make up the ITK Outpatient letter FHIR Document.

When using ITK3 there is an outer bundle structure which is called the [ITK3 send payload bundle structure](https://nhsconnect.github.io/ITK3-FHIR-Messaging-Distribution/explore_messages.html#itk-send-payload-bundle-diagram) for use with ITK3.

<img src="images/explore/outpatientletter_message_bundle.png" style="width: 75%;max-width: 75%;"> 

## Patient ##

The diagram shows the referencing for the Patient resource.

<img src="images/explore/patient_referencing.png" style="width: 75%;max-width: 75%;"> 

## Encounter ##

The diagram shows the referencing for the Encounter resource.

<img src="images/explore/encounter_referencing.png" style="width: 75%;max-width: 75%;"> 

## List (Medication) ##

The diagram shows the referencing for the List resource for Medication.

<img src="images/explore/medication_list_referencing.png" style="width: 75%;max-width: 75%;"> 

## MedicationStatement ##

The diagram shows the referencing for the MedicationStatement resource.

<img src="images/explore/medicationStatement_referencing.png" style="width: 75%;max-width: 75%;">

## Medication ##

The diagram shows the referencing for the Medication resource.

<img src="images/explore/medication_referencing.png" style="width: 50%;max-width: 50%;">  

## Flag (Medication) ##

The diagram shows the referencing for the Flag resource for Medication.

<img src="images/explore/medication_flag_referencing.png" style="width: 75%;max-width: 75%;"> 

## List (Allergy) ##

The diagram shows the referencing for the List resource for Allergies.

<img src="images/explore/allergy_list_referencing.png" style="width: 75%;max-width: 75%;"> 

## AllergyIntolerance ##

The diagram shows the referencing for the AllergyIntolerance resource.

<img src="images/explore/allergyIntolerance_referencing.png" style="width: 75%;max-width: 75%;"> 

## Flag (Allergy) ##

The diagram shows the referencing for the Flag resource for Allergies.

<img src="images/explore/allergy_flag_referencing.png" style="width: 75%;max-width: 75%;"> 

## Condition ##

The diagram shows the referencing for the Condition resource.

<img src="images/explore/condition_referencing.png" style="width: 75%;max-width: 75%;"> 

## Procedure ##

The diagram shows the referencing for the Procedure resource.

<img src="images/explore/procedure_referencing.png" style="width: 75%;max-width: 75%;"> 

## Observation ##

The diagram shows the referencing for the Observation resource.

Note: there are several profiles for the Observation resource.

**Generic ITK Observation**

<img src="images/explore/observation_referencing.png" style="width: 75%;max-width: 75%;"> 

**Occupational History Observation**

<img src="images/explore/occupational_history_observation_referencing.png" style="width: 75%;max-width: 75%;"> 

**Advance Decision to Refuse Treatment Observation**

<img src="images/explore/ADRT_observation_referencing.png" style="width: 75%;max-width: 75%;"> 

**Advance Statement Observation**

<img src="images/explore/advance_statement_observation_referencing.png" style="width: 75%;max-width: 75%;"> 

**Cognition Observation**

<img src="images/explore/cognition_observation_referencing.png" style="width: 75%;max-width: 75%;">

**Lasting Power of Attorney Observation** 

<img src="images/explore/LPoA_observation_referencing.png" style="width: 75%;max-width: 75%;"> 

**Accessible Information Observation** 

<img src="images/explore/accessible_information_observation_referencing.png" style="width: 75%;max-width: 75%;"> 


## Contract ##

The diagram shows the referencing for the Contract resource. 

Note: there are several profiles for the contract resource but they all have a similar structure.

**Advance Statement Contract Profile**
<img src="images/explore/contract_advance_statement_referencing.png" style="width: 75%;max-width: 75%;">

**Advance Decision to Refuse Treatment Profile**
<img src="images/explore/contract_ADRT_referencing.png" style="width: 75%;max-width: 75%;">

**Lasting Power of Attorney Profile**
<img src="images/explore/contract_LPoA_referencing.png" style="width: 75%;max-width: 75%;">

## Practitioner and Organization ##

The diagram shows the referencing between organization, practitioner and practitionerRole.


<img src="images/explore/org_pra_references.png" style="width: 75%;max-width: 75%;"> 
