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
The Examination findings  section carries about the examination and any findings. Elements should be formatted as subheadings in any HTML sent.

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
   <td>Examination finding</td>
   <td>The record of findings from clinical examination.</td>
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
   <td>Examination</td>
   <td>This could include site and must include laterality where applicable.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>This is the record of the examinations undertaken during the appointment. Text or coded text (SNOMED CT).The examination performed, eg general appearance, vital signs, mental state, head and neck examination, oral examination, cardiovascular system, respiratory system, abdomen, genitourinary, nervous system, musculoskeletal system, skin.</td>
  </tr>
  <tr>
   <td>Examination findings</td>
   <td>The record of findings from the examinations performed.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>This is the record of clinically relevant findings from the examinations undertaken during the appointment. Text or coded text (SNOMED CT).</td>
  </tr>
 </tbody>
</table>


##  Example Examination Findings Section ##

<script src="https://gist.github.com/IOPS-DEV/d39ad2e1297ea67df7488910d97d4a3b.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format. See constructing coded clinical structures 


- [Condition](build_conditions.html)
- [Observation](build_observations.html)






