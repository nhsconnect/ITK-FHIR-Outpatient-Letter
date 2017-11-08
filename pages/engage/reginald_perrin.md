---
title: Reginald Perrin Outpatient Letter Scenario
keywords: workflow
tags: [development,fhir,profiles]
sidebar: overview_sidebar
permalink: engage_reginald_perrin.html
summary: "Example scenario - Reginald Perrin Outpatient Letter"
---

{% include custom/search.warnbanner.html %}

## Background ##
Reginald attends an outpatient appointment at St Crispin’s Hospital having been previously referred by Michael McMonagle who is the Occupational Therapist at the Head Injury Team of St Crispin’s Hospital.Reginald was experiencing diplopia.

## The Outpatient Encounter ##

The Outpatient encounter carried in the [Encounter Resource](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-ITK-Encounter-1)

## Named Participants ##

- Patient - **Mr. Reginald Perrin** - [Patient Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Patient-1)
- Orthoptist (Document author) - **Rupert Rigsby** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Patient's GP (Document recipient) - **Dr  C. O’Reilly** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Occupational Therapist (Document recipient and original referrer) - **Michael McMonagle** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
## Named Organisations ##

- Patient's GP Practice - **Canvas Health Centre** - [Organization Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Organization-1)
- Hospital - **St Crispin’s Hospital** - [Organization Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Organization-1)


During the Outpatients encounter Robert diagnoses Reginald with Right hypertropia and fits a prism to his glasses to relieve it.
He refers Reginald to an ophthalmologist. He also advises him to inform the DVLA regarding the diplopia and fresnel prism. 


## Example Instance of Scenario ##

<script src="https://gist.github.com/IOPS-DEV/f137046205ee2da61ce36e24e19ca8fc.js"></script>

## Example Rendered Instance of Scenario ##

This is a rendered example of the above XML example using an [exemplar stylesheet](https://github.com/nhsconnect/ITK3-FHIR-Documents-Renderer/tree/develop) created by NHS Digital. This style is currently draft and available for use on a AS IS BASIS. 

Due to the size of the image, this example is best viewed with the navigation side bar switched off <img src="images/engage/nav_shot.png" style="width:8%;max-width: 8%;">.

<img src="images/engage/reginald_01.png" style="width:100%;max-width: 100%;">