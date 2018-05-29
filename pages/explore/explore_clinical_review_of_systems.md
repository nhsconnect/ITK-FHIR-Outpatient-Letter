---
title: Clinical Review of Systems Section
keywords:  messaging, sections
tags: [fhir,messaging,sections]
sidebar: foundations_sidebar
permalink: explore_clinical_review_of_systems.html
summary: "Gives information about the Clinical review of systems section"
---

{% include custom/section.warnbanner.html %}

## Clinical Review of Systems Section Content##
The Clinical review of systems section carries a narrative summary of the information gathered on symptoms related to physiological systems where possible, very brief. Elements should be formatted as sub headings in any HTML sent.

<table style="width:100%;max-width: 100%;">
	<thead>
		<tr>
			<th width="18%">Section</th>
			<th width="30%">Description</th>
			<th width="11%">Cardinality</th>
			<th width="11%">MRO*</th>
			<th width="30%">Values</th>
		</tr>
	</thead>
 <tbody>
  <tr>
   <td>Clinical review of systems</td>
   <td>Information gathered on symptoms related to physiological systems.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>&nbsp;</td>
  </tr>
		<tr>
			<th>Element</th>
			<th>Description</th>
			<th>Cardinality</th>
			<th>MRO*</th>
			<th>Values</th>
		</tr>
  <tr>
   <td>Clinical review of systems</td>
   <td>The clinical review of systems. The record of clinical information gathered in responses to questions to the patient about general symptoms from various physiological systems, including food intake (increasing/decreasing) weight change, swallowing difficulties etc.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>This is the record of the review of systems as volunteered by the patient or their representative or carer. Text or coded text (SNOMED CT).</td>
  </tr>
 </tbody>
</table>

##  Example Clinical Review of Systems Section ##

<script src="https://gist.github.com/IOPS-DEV/cf4cfb8d434264587ffd5d5b03998c50.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK3 FHIR Outpatient Letter does not currently support coded clinical review of systems information.






