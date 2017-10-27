---
title: Diagnoses Section
keywords:  messaging, sections
tags: [fhir,messaging,section]
sidebar: foundations_sidebar
permalink: explore_diagnoses.html
summary: "Gives information about the Diagnoses section"
---

{% include custom/section.warnbanner.html %}

## Diagnoses Section Content##
The Diagnoses section carries information about Diagnoses, items in bold are subheadings and should be formatted as such in any html sent:

- **Diagnosis** - Confirmed diagnosis (or symptom); active diagnosis being treated.
- **Stage** - Stage of the disease, where relevant
- **Comment** - Supporting text may be given covering diagnosis confirmation, active diagnosis being treated.


##  Example Diagnoses Section ##

This section example includes a reference to a coded diagnosis.

<script src="https://gist.github.com/IOPS-DEV/6903725738cefc330a8964316f0a5e9d.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- Condition
 
See constructing coded clinical structures - [Condition](build_conditions.html)






