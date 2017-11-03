---
title: Ophelia Gently Outpatient Letter Scenario
keywords: workflow
tags: [development,fhir,profiles]
sidebar: overview_sidebar
permalink: engage_ophelia_gently.html
summary: "Example scenario - Ophelia Gently Outpatient Letter"
---

{% include custom/search.warnbanner.html %}

## Background ##
Miss Gently was referred to the rheumatology outpatient clinic by her GP due to multiple joint pain which was causing her to not sleep well. She has previously been diagnosed with Type 1 diabetes and hypothyroidism. 

## The Outpatient Encounter ##

The Outpatient encounter carried in the [Encounter Resource](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-ITK-Encounter-1)

## Named Participants ##

- Patient - **Ophelia Gently** - [Patient Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Patient-1)
- Consultant Rheumatologist (Document Author) - **Dr. H.H. Crippen** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Patient's GP (Document recipient) - **Dr.  C. O’Reilly** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)

## Named Organisations ##

- Patient's GP Practice - **Canvas Health Centre** - [Organization Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Organization-1)
- Discharging Hospital - **St Crispin’s Hospital** - [Organization Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Organization-1)

During the consultation Ophelia explains to Dr. Crippen that she wants not to be in constant pain so she can get a good nights sleep and that she is fed up will being tired all the time. The Dr. Crippen tells Ophelia that her tests all came back normal and that he wants to change her medication. He believes that Amitriptyline should be prescribed and explains that this should help her sleep much better. He also tells Ophelia that she should try to take regular gentle exercise and to gradually increase the amount. He advises her that the previous abnormal blood results are not of any  significant other than reflecting her known diagnosis of thyroid disease.
He writes her a prescription for two weeks supply of Amitriptyline explaining that she need to take it about an hour before going to bed. He says that he will instruct her GP to prescribe more after the first two weeks course.

## Example Instance of Scenario ##

<script src="https://gist.github.com/IOPS-DEV/7f7b6a3aa15ac1465cfe9c10256d7531.js"></script>

## Example Rendered Instance of Scenario ##

This is a rendered example of the above XML example using an [exemplar stylesheet](https://github.com/nhsconnect/ITK3-FHIR-Documents-Renderer/tree/develop) created by NHS Digital. This style is currently draft and available for use on a AS IS BASIS. 

Due to the size of the image, this example is best viewed with the navigation side bar switched off <img src="images/engage/nav_shot.png" style="width:8%;max-width: 8%;">.

<img src="images/engage/ophelia_01.png" style="width:100%;max-width: 100%;">



