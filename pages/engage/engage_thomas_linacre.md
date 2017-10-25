---
title: Thomas Linacre Outpatient Letter Scenario
keywords: workflow
tags: [development,fhir,profiles]
sidebar: overview_sidebar
permalink: engage_thomas_linacre.html
summary: "Example scenario - Thomas Linacre Outpatient Letter"
---

{% include custom/search.warnbanner.html %}

## Background ##
Mr. Tom Linacre attends an outpatient appointment at St Crispin’s Hospital having been previously referred by Sugra Bibi. This was because Tom was recently readmitted to hospital following a stroke which left him with swallowing difficulties. During the hospital stay Mr. Linacre was established on a PEG tube feeding. The feeding tube insitu is a 15French PEG tube placed 05/04/17. The regimen being: 1000mls Energy Multifibre Feed at 100mls/hours for 10 hours (9am-7pm) with 1400mls water given as divided flushes (e.g. 10x140mls) throughout the day e.g. before and after feed and with medications. 

## The Outpatient Encounter ##

The Outpatient encounter carried in the [Encounter Resource](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-ITK-Encounter-1)

## Named Participants ##

- Patient - **Mr. Thomas  (Tom) Linacre** - [Patient Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Patient-1)
- Community Dietician (Document author) - **Susan Blight** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Patient's GP (Document recipient) - **Dr  C. O’Reilly** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Feeding nurse (Document recipient) - **Doug Sway** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Hospital Dietician (Document recipient and original referrer) - **Sugra Bibie** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Neurologist (Document recipient) - **Dr. Gerald McManus** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)

## Named Organisations ##

- Patient's GP Practice - **Canvas Health Centre** - [Organization Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Organization-1)
- Hospital - **St Crispin’s Hospital** - [Organization Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Organization-1)
- Feed Company (Document Recipient) - **Company  X** - [Organization Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Organization-1)

During the Outpatients encounter Susan Blight measures Tom's weight, height and BMI. she asks Tom how he is coping with his feed and tube. Tom says he is managing ok and doing all he has been instructed to do. Susan examines Tom's peg site an notes that it has healed well and is clean and dry. Susan asks Tom if his bowel movements are good, to which Tom replies that his bowels are opening daily without any medication.
Susan revises his medication and decides that Tom needs 100ml/day of energy fibre feed given via PEG tube over 10hrs (10am-7pm). 1400mls water given as divided flushes (e.g. 10x140mls) throughout the day e.g. before and after feed and with medications.
She tells Tom that she will advise the GP to prescribe 28 x 100ml bags per month, the prescription to be sent directly to the feed company who will deliver direct to Tom.

Susan tells Tom she will request a Feeding Company Nurse to train Tom on use of pump.
She also tells him she will order a backpack so that Tom can feed when he goes out during the day as he did not like feeding during the night when he was in hospital and feels restricted to stay at home at the moment.
Susan asks Tom to continue on the feeding regime and gives the clinic contact details and a copy of his feeding regime with Trust guidance.


## Example Instance of Scenario ##

<script src="https://gist.github.com/IOPS-DEV/e34faf1969470b219b403b98df66593c.js"></script>