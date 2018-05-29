---
title: Work flow
keywords: workflow
tags: [development,fhir,profiles]
sidebar: overview_sidebar
permalink: workflow_encounter.html
summary: "Overview of the work flow using Encounter Resource."
---

{% include custom/search.warnbanner.html %}

## Overview ##

The Outpatient Letter does not support any real "work flow" but uses the encounter Resource to give context to the information contained in the Outpatient Letter document. The encounter Resource represents the Outpatient appointment and can contain important information such as:
 
- When the patient attended the appointment
- Why the patient attended the appointment
- Who was involved in the appointment

The encounter can be referenced by the following resources:

- Composition
- Condition 
- List
- MedicationStatement
- Procedure

## Example Encounter ##

<script src="https://gist.github.com/IOPS-DEV/66bff9022f16f8341ec1f7b77391ac23.js"></script>




