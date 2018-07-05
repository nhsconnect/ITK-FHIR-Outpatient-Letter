---
title: Sam Beckett Outpatient Letter Scenario
keywords: workflow
tags: [development,fhir,profiles]
sidebar: overview_sidebar
permalink: engage_sam_beckett.html
summary: "Example scenario - Sam Beckett Outpatient Letter Scenario"
---



## Background ##
Sam who is a Polish national attends an Outpatient appointment at St Crispin’s Hospital having been referred by Dr. William Yates who is a Dermatology Consultant at St Crispin’s Hospital. She has a potential Squamous cell carcinoma to the left forearm. She has had a rapidly growing lesion to left forearm for last 10 months. She has seen dermatologists who have assessed and referred on to Plastics for surgical excision and possible skin grafting after the lesion is excised. Sam's father died of melanoma at 62 years old. Sam lives with her husband. She is a factory worker, does not smoke and her alcohol intake is rare.

## The Outpatient Encounter ##

The Outpatient Encounter carried in the [Encounter Resource](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-ITK-Encounter-1)

## Named Participants ##

- Patient - **Mrs. Sam Beckett** - [Patient Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Patient-1)
- Consultant surgeon (Document author) - **Dr. Shauna O’Casey** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Skin cancer specialist nurse (Assisting Care professional) - **Patricia Kavanagh** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Health care assistant (Care professional present) - **Jane Joyce** - - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Patient's GP (Document recipient) - **Dr  C. O’Reilly** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)

## Named Organisations ##

- Patient's GP Practice - **Canvas Health Centre** - [Organization Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Organization-1)
- Hospital - **St Crispin’s Hospital** - [Organization Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Organization-1)

During the Outpatient Encounter Dr. Shauna O’Casey notes that Sam is a Polish national and speaks little English. He examines her arm and notes that there are no skin lesions to the body other than left forearm. She has a 3x2cm scaly lesion which is centrally ulcerated. There was no evidence of left axillary or cervical node involvement. She is warned about the risk of infection, bleeding, re-operation, scarring, wound dehiscence and the need for dressings. This is important as Sam is allergic Penicillin which causes nausea and vomiting. She understands this and is happy to be added to the waiting list for a excisional biopsy of lesion and direct closure on left forearm by Dr. Shauna O’Casey. 

## Example Instance of Scenario ##

<script src="https://gist.github.com/IOPS-DEV/3a2e612aabb55a54f885767236de9da6.js"></script>

