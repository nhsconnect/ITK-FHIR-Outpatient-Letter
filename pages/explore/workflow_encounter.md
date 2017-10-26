---
title: Work flow
keywords: workflow
tags: [development,fhir,profiles]
sidebar: overview_sidebar
permalink: workflow_encounter.html
summary: "Overview of work flow using encounter resource."
---

{% include custom/search.warnbanner.html %}

## Overview ##

The Outpatient letter does not support any real "workflow" but uses the encounter resource to give context to the information contained in the Outpatient letter document. The encounter resource represent the Outpatient encounter and can contain important information such as:
 
- When the patient attended
- Why the patient attended
- Follow-up information
- Who was involved in the encounter
- How the encounter ended, referrals, etc 

The encounter can be referenced by the following resources:

- Composition
- Condition 
- Flag
- List
- MedicationStatement
- Observation
- Procedure

## Example Encounter ##

<script src="https://gist.github.com/IOPS-DEV/17df2fb7810e062d2df64afa3aecea40.js"></script>




