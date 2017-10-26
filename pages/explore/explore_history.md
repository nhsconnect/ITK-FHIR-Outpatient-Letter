---
title: History Section
keywords:  messaging, sections
tags: [fhir,messaging,sections]
sidebar: foundations_sidebar
permalink: explore_history.html
summary: "Gives information about the History section"
---

{% include custom/section.warnbanner.html %}

## History Section Content##
The History section carries history related to the patient's previous care, items in bold are subheadings and should be formatted as such in any html sent:

- **Patient’s reason for referral**	- Patient stated reason for referral. This may include any discussions that took place, the level of shared decision making involved, information about patient’s source of advice. This may be expressed on behalf of the patient, eg by parent or carer.
- **Presenting complaint or issue**	- The list and description of the health problems and issues experienced by the patient resulting in the attendance. This may include disease state, medical condition, response and reaction to therapies, eg blackout, dizziness, chest pain, follow-up from admission, falls, a specific procedure, investigation or treatment.
- **History of each presenting complaint or issue**	- Information directly related to the development and characteristics of each presenting complaint (eg including travel history). Including if the information is given by the patient or their carer.	
- **History since last contact** - History since last attendance, discharge from hospital, etc. To include adherence to treatment plan, where appropriate.
- **Relevant past medical, surgical and mental health history** -The record of the person’s significant medical, surgical and mental health history. Including relevant previous diagnoses, problems and issues, procedures, investigations, specific anaesthesia issues, etc (will include dental and obstetric history)	


##  Example History Section ##

<script src="https://gist.github.com/IOPS-DEV/dad7e1028c8a046c3dbe44d03ef6c6fb.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- [Condition](build_conditions.html)
- [Observation](build_observations.html)
- [Procedure](build_procedures.html)





