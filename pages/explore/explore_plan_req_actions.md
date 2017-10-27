---
title: Plan and requested actions Section
keywords:  messaging, sections
tags: [fhir,messaging,section]
sidebar: foundations_sidebar
permalink: explore_plan_req_actions.html
summary: "Gives information about the Plan and requested actions section"
---

{% include custom/section.warnbanner.html %}

## Plan and Requested Actions Content ##
The Plan and requested actions section carries information about planned and requested actions such as planned investigations, procedures etc, items in bold are subheadings and should be formatted as such in any html sent:

- **Actions for healthcare professionals** - 	Including planned investigations, procedures and treatment for a patient’s identified conditions and priorities. For each action the following should be identified:
	- person responsible - name and designation / department / hospital etc or role (eg GP) responsible for carrying out the proposed action, and where action should take place**
	- status - requested, planned or completed
	- When action requested for - requested date, time, or period - as relevant
	- suggested strategies - suggested strategies for potential problems,
	- outcome expectations, including patient’s expectations
- **Actions for patient or their carer** - For each action the following should be identified:
	- person responsible - name and designation eg patient or carer responsible for carrying out the proposed action, and where action should take place
	- status - requested, planned or completed
	- When action requested for - requested date, time, or period - as relevant
	- suggested strategies - suggested strategies for potential problems, eg telephone contact for advice
	- outcome expectations, including patient’s expectations.
- **Agreed with patient or legitimate patient representative** - Indicates whether the patient or legitimate representative has agreed the entire plan or individual aspects of treatment, expected outcomes, risks and alternative treatments.
- **Care planning arrangements** - Record if CPA (Care Programme Approach) documentation is available and how and where it can be accessed; care and treatment plan in Wales and Scotland. In Wales this is superseded by the Mental Health Measure 2010.


##  Example Plan and Requested Actions Section ##

<script src="https://gist.github.com/IOPS-DEV/e60a0b729371552cca12038570d52ca8.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK FHIR Outpatient letter does not currently support coded Plan and requested actions information.






