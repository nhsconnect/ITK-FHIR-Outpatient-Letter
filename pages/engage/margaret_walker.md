---
title: Margaret Walker Outpatient Letter Scenario
keywords: workflow
tags: [development,fhir,profiles]
sidebar: overview_sidebar
permalink: engage_margaret_walker.html
summary: "Example scenario - Margaret Walker Outpatient Letter"
---

{% include custom/search.warnbanner.html %}

## Background ##
Margaret attends an appointment at St Crispin’s Hospital palliative care Outpatient clinic accompanied by her daughter Karen. Margaret was referred for review of symptom control.

 Margaret has been on pazopanib since May 2017. She had a right nephrectomy for clear cell renal carcinoma in Sept 2016, and now has metastatic disease. Margaret struggles with pain predominantly around the right upper quadrant of her abdomen and this goes all the way round to the back, at worst described as 10/10.  She has been reluctant to take full dose of Co-codamol and she intermittently takes one tablet at a time (30/500mg). Karen believes her mother has a high pain tolerance level and tends to underplay her symptoms. Margaret finds herself tiring out by the second half of the day, particularly if she has done a bit more than usual earlier on. 
 
Karen and her mother have been intermittently tearful and upset given news of disease recurrence and are doing their best to deal with it. Margaret wasn’t expecting to hear about cancer recurrence in such a short period after her surgery.

## The Outpatient Encounter ##

The Outpatient encounter carried in the [Encounter Resource](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-ITK-Encounter-1)

## Named Participants ##

- Patient - **Margaret Walker** - [Patient Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Patient-1)
- Patient's daughter (present during encounter) - **Karen Walker** - [RelatedPerson Resource](https://fhir.nhs.uk/STU3/StructureDefinition/ITK-RelatedPerson-1)
- IBD specialist nurse (Care professional present) - **Mrs. N Bryant** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Consultant in Palliative Medicine (Document author) - **Dr. Doris Mackay** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Medical Oncologist (Document recipient) - **Professor Hawkins** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Community Macmillan Team member (Document recipient) - **Susan Snodgrass** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Patient's GP (Document recipient) - **Dr  C. O’Reilly** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)

## Named Organisations ##

- Patient's GP Practice - **Canvas Health Centre** - [Organization Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Organization-1)
- Hospital - **St Crispin’s Hospital** - [Organization Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Organization-1)

During the Outpatient encounter Margaret is very clear that she wishes to have as much detail as possible and asked about her prognosis. She does not wish to be resuscitated in the event of a cardio respiratory arrest. 

Doris discusses with Margaret and her daughter the benefit of being able to do more through the day and having better psychological well-being when pain is better controlled. She has explained how they would use long acting Morphine preparation along with Oramorph to get control of background as well as breakthrough cancer pain. Given the degree of tenderness around the subcutaneous nodule on the right upper quadrant, they discussed that radiotherapy may be helpful with the pain.

Doris discusses that Margaret's fatigue is part of the cancer presentation, and they discuss being pragmatic - doing activities with gaps in between to allow herself to conserve energy whilst pacing herself through the day.  Doris encourages her to cut back on tasks that are not as important as others such as her household chores and to delegate them to others, such as family where possible. She acknowledged that this is a significant change in her lifestyle given that Margaret was independently managing everything for a long time.

Doris explains that while the speed at which disease recurrence has happened doesn’t bode well, they will need to see how Margaret is likely to respond to potential treatment options.  They are likely to know more about prognosis following her appointment with the Oncologist in the next couple of weeks - They don’t know how she will respond to treatment in itself. It may be that the treatment might be effective but that she might not be strong enough to cope with it on a long term basis; however she is hopeful that there will be some positive outcome with the treatment.  Doris encourages Margaret to proceed with planning ahead and deciding about what she would prefer to happen irrespective of her prognosis.

Doris agrees that Margaret's wish not to be resuscitated in the event of a cardio respiratory arrest was sensible and advises her either she or or herself could complete a community DNACPR form in the near future. Margaret indicates that her son and daughter are aware that she could have an appointed LPA on matters of her health and well-being. She is considering funeral arrangement plans.

Doris arranges for Margaret to see Professor Hawkins for consideration of immunotherapy as it is hopeful that she will have some benefit from this treatment. Currently her performance status is around 1-2. Professor Hawkins is requested to consider radiotherapy to help with pain as a result of degree of tenderness around the subcutaneous nodule on the right upper quadrant.

Doris gives Margaret prescriptions for new medications and tells her that she can get in touch with her if there are any concerns.


## Example Instance of Scenario ##

<script src="https://gist.github.com/IOPS-DEV/4f07e9048566cbee14245ad6dea35e9d.js"></script>

