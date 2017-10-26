---
title: Examination Findings Section
keywords:  messaging, sections
tags: [fhir,messaging,sections]
sidebar: foundations_sidebar
permalink: explore_examination_findings.html
summary: "Gives information about the Examination findings section"
---

{% include custom/section.warnbanner.html %}

## Examination Findings Section Content##
The Examination findings  section carries about the examination and any findings, items in bold are subheadings and should be formatted as such in any html sent:

- **Examination**	The examination performed, eg general appearance, vital signs, mental state, head and neck examination, oral examination, cardiovascular system, respiratory system, abdomen, genitourinary, nervous system, musculoskeletal system, skin.This is the record of the examinations undertaken during the appointment. 		
- **Examination findings**	The record of findings from the examinations performed. This is the record of clinically relevant findings from the examinations undertaken during the appointment.

##  Example Examination Findings Section ##

<script src="https://gist.github.com/IOPS-DEV/d39ad2e1297ea67df7488910d97d4a3b.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format. See constructing coded clinical structures 


- [Condition](build_conditions.html)
- [Observation](build_observations.html)






