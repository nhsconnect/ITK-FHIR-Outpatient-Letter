---
title: Sam Beckett Outpatient Letter Scenario
keywords: workflow
tags: [development,fhir,profiles]
sidebar: overview_sidebar
permalink: engage_sam_beckett.html
summary: "Example scenario - Sam Beckett Outpatient Letter Scenario"
---

{% include custom/search.warnbanner.html %}

## Background ##
Sam who is a Polish national attends an outpatient appointment at St Crispin’s Hospital having been referred by Dr. William Yates who is a Dermatology Consultant at St Crispin’s Hospital. She has a potential Squamous cell carcinoma to left forearm. Rapidly growing lesion to left forearm x 10 months. She has seen dermatologists who have assessed and referred on to Plastics for surgical excision and possible skin grafting after lesion is excised. Sam father died of melanoma at 62year old. Sam lives with her husband. She is a factory worker, does not smoke and her alcohol intake is rare.

## The Outpatient Encounter ##

The Outpatient encounter carried in the [Encounter Resource](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-ITK-Encounter-1)

## Named Participants ##

- Patient - **Mrs. Sam Beckett** - [Patient Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Patient-1)
- Consultant surgeon (Document author) - **Dr. Shauna O’Casey** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Skin cancer specialist nurse (Assisting Care professional) - **Patricia Kavanagh** - - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Health care assistant (Care professional present) - **Jane Joyce** - - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Patient's GP (Document recipient) - **Dr  C. O’Reilly** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)

## Named Organisations ##

- Patient's GP Practice - **Canvas Health Centre** - [Organization Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Organization-1)
- Hospital - **St Crispin’s Hospital** - [Organization Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Organization-1)

During the Outpatients encounter Dr. Shauna O’Casey notes that Sam is a Polish national and speaks little English. He examines her arm and notes that there are no skin lesions to the body other than left forearm. She has a 3x2cm scaly lesion which is centrally ulcerated. There was no evidence of left axillary or cervical node involvement. She is warned about the risk of infection, bleeding, re-operation, scarring, wound dehiscence and the need for dressings. This is important as Sam is allergic Penicillin which causes nausea and vomiting. She understands this and is happy to be added to the waiting list for a excisional biopsy of lesion and direct closure on left forearm by Dr. Shauna O’Casey. 

## Example Instance of Scenario ##

<script src="https://gist.github.com/IOPS-DEV/3a2e612aabb55a54f885767236de9da6.js"></script>

## Example Rendered Instance of Scenario ##

This is a rendered example of the above XML example using an [exemplar stylesheet](https://github.com/nhsconnect/ITK3-FHIR-Documents-Renderer/tree/develop) created by NHS Digital. This style is currently draft and available for use on a AS IS BASIS. 

Due to the size of the image, this example is best viewed with the navigation side bar switched off <img src="images/engage/nav_shot.png" style="width:8%;max-width: 8%;">.

<img src="images/engage/sam_01.png" style="width:100%;max-width: 100%;">