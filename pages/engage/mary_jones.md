---
title: Mary Jones Outpatient Letter Scenario
keywords: workflow
tags: [development,fhir,profiles]
sidebar: overview_sidebar
permalink: engage_mary_jones.html
summary: "Example scenario - Mary Jones Outpatient Letter"
---

{% include custom/search.warnbanner.html %}

## Background ##
Mary attends an outpatient appointment at St Crispin’s Hospital with her mother, for scheduled review of tonic-clonic seizures and gastro-oesophageal reflux. Mary has been well. However she is now having on average four tonic-clonic seizures a day. Her mother has had to give her rectal diazepam on two occasions but she has not needed to go to hospital. She had a PEG inserted in April 2017 and her reflux has reduced considerably since then. Mary has increasing spasticity of right hip and more frequent tonic-clonic convulsions. Mary started at Greenacre School in September. She enjoys it and the teachers are pleased with her progress.  Her mother has been bringing her to school by car, but this is becoming an increasing problem as due to recent changes at work she now has to start work at 8:30 AM. Unfortunately Mary is not eligible for free school transport until she is five years old. The home-school liaison teacher is trying to come to an agreement with the local authority to enable Mary to use school transport.  The teacher for visual impairment has seen her in school and recommended that she use large print books and a magnifying glass.

## The Outpatient Encounter ##

The Outpatient encounter carried in the [Encounter Resource](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-ITK-Encounter-1)

## Named Participants ##

- Patient - **Mary Jones** - [Patient Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Patient-1)
- Patient's mother (Document recipient and present during encounter) - **Sally Jones** - [RelatedPerson Resource](https://fhir.nhs.uk/STU3/StructureDefinition/ITK-RelatedPerson-1)
- Patient's father (Document recipient) - **Ian Jones** - [RelatedPerson Resource](https://fhir.nhs.uk/STU3/StructureDefinition/ITK-RelatedPerson-1)
- Consultant paediatrician (Document author) - **Dr. Arnold Rimmer** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Occupational therapist (Care professional present) - **Jenny White** - - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Health care assistant (Care professional present) - **Sarah Hall** - - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Consultant orthopaedic (Document recipient) - **Dr. Charlotte Worth** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Epilepsy nurse (Document recipient) - **Philip Brown** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Patient's GP (Document recipient) - **Dr  C. O’Reilly** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)

## Named Organisations ##

- Patient's GP Practice - **Canvas Health Centre** - [Organization Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Organization-1)
- Hospital - **St Crispin’s Hospital** - [Organization Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Organization-1)

During the Outpatient encounter a Neurodevelopmental assessment is done which finds that Mary can now sit unsupported for about 30 seconds. When lying prone she can draw her knees up underneath her but does not make any attempts to move. In clinic she was able to complete the circle and square form board but cannot do them reversed. She can say 10 words with meaning and her mother feels she can understand far more. She is able to finger feed and will drink from a cup if it is held for her. She is becoming more sociable and has a lovely smile. 

An examination determines that Mary's ankles both dorsiflex to 90°.  Her hips are very tight; the right hip only abducts to 30° and the left hip to 45°. The right hip has deteriorated.
No evidence of dental caries. Dr Rimmer requests to orthopaedics for early appointment for advice on deteriorating right hip. He also gives Mary's mother a letter of support to education regarding school transport.  Dr Rimmer then reviews Mary's medication and changes the dose quantities .He asks Mary's mother to review Mary's medication by phone in two weeks with Phil Brown who is a epilepsy nurse.
 

## Example Instance of Scenario ##

<script src="https://gist.github.com/IOPS-DEV/944c204f72f37498bb72797d2e391b84.js"></script>

