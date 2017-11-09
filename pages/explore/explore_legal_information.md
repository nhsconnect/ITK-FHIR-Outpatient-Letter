---
title: Legal Information Section
keywords:  messaging, sections
tags: [fhir,messaging,section]
sidebar: foundations_sidebar
permalink: explore_legal_info.html
summary: "Gives information about the Legal information section"
---

{% include custom/section.warnbanner.html %}

## Legal Information Section Content ##
The Legal information section carries information about legal information perinatal to the patient,items in bold are subheadings and should be formatted as such in any html sent:

- **Consent for information sharing** - This is a record of consent for information sharing. Where consent has been not been obtained or sought, the reason why must be provided. Include best interests decision where person lacks capacity.
- **Consent relating to child**	- Consideration of age and competency. Record of person with parental responsibility or appointed guardian where child lacks competency.	
- **Mental capacity assessment** -	Whether an assessment of the mental capacity of the (adult) person has been undertaken, if so, what capacity the decision relates to, who carried it out, when and the outcome of the assessment. Also record best interests decision if person lacks capacity.
- **Deprivation of Liberty Safeguards or equivalent** -	Record of Deprivation of Liberty Safeguards (DoLS) or equivalent, including the reason for this.
- **Mental Health Act or equivalent status** -	Record where a person diagnosed with a mental disorder is formally detained under the Mental Health Act or equivalent, including the section number and start date, start time and end date. If person subject to Community Treatment Order or Conditional Discharge (or equivalent) record here.
- **Advance decision to refuse treatment (ADRT)**	A record of an advance decision to refuse one or more specific types of future treatment, made by a person who had capacity at the time of recording the decision. The decision only applies when the person no longer has the capacity to consent to or refuse the specific treatment being considered. An ADRT must be in writing, signed and witnessed. If the ADRT is refusing life-sustaining treatment it must state specifically that the treatment is refused even if the person’s life is at risk. Where available a copy of the ADRT may be appended to the record. Where there has been a change in the ADRT this should be noted in the record in free text.
- **Lasting power of attorney  for personal welfare  or court-appointed deputy (or equivalent)**	- Record of one or more people who have been given power (LPA) by the person when they had capacity to make decisions about their health and welfare should they lose capacity to make those decisions. To be valid, an LPA must have been registered with the Court of Protection. If life-sustaining treatment is being considered the LPA document must state specifically that the attorney has been given power to consent to or refuse life-sustaining treatment. Details of any person (deputy) appointed by the court to make decisions about the person’s health and welfare. A deputy does not have the power to refuse life-sustaining treatment. The name of the LPA should be recorded. The authority of the LPA should be recorded as SNOMED CT codes (see National Information Standard (SCCI1580) and associated text. The contact details of the LPA should be recorded under the relevant contacts heading.
- **Legal safeguarding issues**	Any legal matters relating to safeguarding of a vulnerable child or adult, e.g., child protection plan, protection of vulnerable adult.	

## Example Legal Information Section ##

<script src="https://gist.github.com/IOPS-DEV/38688357710decd6e80bc597a9da54e2.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- [Contract(ADRT and LPOA)](build_contracts.html)
- [Observation(ADRT and LPOA)](build_observations.html)







