---
title: Agatha Critchard Outpatient Letter Scenario
keywords: workflow
tags: [development,fhir,profiles]
sidebar: overview_sidebar
permalink: engage_agatha_critchard.html
summary: "Example scenario - Agatha Critchard Outpatient Letter"
---

{% include custom/search.warnbanner.html %}

## Background ##
Agatha attends an outpatient appointment at St Crispin’s Hospital having been previously referred by her GP. Agatha has ongoing symptoms of bloody diarrhoea, weight loss, and abdominal discomfort that are unresponsive to treatment.  She has a 2 month history of bloody diarrhoea. Her bowels open 5-6 per day with 1-2 nocturnal episodes. Agatha has experienced weight loss of 1 stone over the same period. She experiences a crampy left iliac fossa pain intermittently. She has no history of travel, unwell contacts or previous similar symptoms. She has longstanding mild dyspepsia for which she takes antacid as necessary. It has never been investigated. Agatha lives with her boyfriend and works as a Baker. She is an ex-smoker, stopped 2 years, and consumed 10-14 units of alcohol per week. Agatha has an allergic reaction to Amoxicillin, which presents as an urticarial rash in the form of a generalized severe rash. She first experienced a reaction aged 12 and has been told the probability of recurrence is likely.

## The Outpatient Encounter ##

The Outpatient encounter carried in the [Encounter Resource](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-ITK-Encounter-1)

## Named Participants ##

- Patient - **Ms. Agatha Crtichard** - [Patient Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Patient-1)
- Consultant Gastroenterologist (Document author) - **Dr. Ruth Jones** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- IBD specialist nurse - **Mrs. N Bryant** - - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Patient's GP (Document recipient) - **Dr  C. O’Reilly** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)

## Named Organisations ##

- Patient's GP Practice - **Canvas Health Centre** - [Organization Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Organization-1)
- Hospital - **St Crispin’s Hospital** - [Organization Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Organization-1)

During the Outpatients encounter Ruth performs a Rigid sigmoidoscopy with the assistance of nurse Bryant to the limit of view at 20cm. Which shows inflamed and ulcerated mucosa with contact bleeding to about 15cm. Proximally appears to improve. The abdomen was found to be soft but mainly tender in the left iliac fossa. There was no guarding or rebound and bowel sounds normal. 

Ruth findings suggest IBD. She changes Agatha's medication and wants the treatment to  commence today pending further investigation. She requests that a flexible sigmoidoscopy is done on an urgent basis. FBC, U&E, LFT and CRP are to be measured. Agatha is asked to provide Stool samples and given the forms and instructions how to do this.


## Example Instance of Scenario ##

<script src="https://gist.github.com/IOPS-DEV/5b51bd5e3814ebca8323f57fde21bbec.js"></script>

## Example Rendered Instance of Scenario ##

This is a rendered example of the above XML example using an [exemplar stylesheet](https://github.com/nhsconnect/ITK3-FHIR-Documents-Renderer/tree/develop) created by NHS Digital. This style is currently draft and available for use on a AS IS BASIS. 

Due to the size of the image, this example is best viewed with the navigation side bar switched off <img src="images/engage/nav_shot.png" style="width:8%;max-width: 8%;">.

<img src="images/engage/agatha_01.png" style="width:100%;max-width: 100%;">
