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
The Examination findings  section carries about the examination and any findings. PRSB Elements should be formatted as subheadings in any HTML sent.
<table style="width:100%;max-width: 100%;">
	<thead>
		<tr>
			<th width="15%">Section</th>
			<th width="35%">Description</th>
			<th width="5%">Card.</th>
			<th width="5%">MRO*</th>
			<th width="40%">FHIR Target and Guidance</th>
		</tr>
	</thead>
 <tbody>
  <tr>
   <td>Examination finding</td>
   <td>The record of findings from clinical examination.</td>
   <td>0 to 1</td>
   <td>O</td>
   <td>Carried in the CodeableConcept of <b>Composition.section.code</b> FHIR element.</td>
  </tr>
		<tr>
			<th>PRSB Element</th>
			<th>Description</th>
			<th>Card.</th>
			<th>MRO*</th>
			<th>FHIR Target and Guidance</th>		
		</tr>
  <tr>
   <td>Examination</td>
   <td>This could include site and must include laterality where applicable.</td>
   <td>0 to 1</td>
   <td>O</td>
   <td>Carried as text only, this is the record of the examinations undertaken during the appointment. The examination performed, eg general appearance, vital signs, mental state, head and neck examination, oral examination, cardiovascular system, respiratory system, abdomen, genitourinary, nervous system, musculoskeletal system, skin.</td>
  </tr>
  <tr>
   <td>Examination findings</td>
   <td>The record of findings from the examinations performed.</td>
   <td>0 to 1</td>
   <td>O</td>
   <td>This is the record of clinically relevant findings from the examinations undertaken during the appointment. Text only.</td>
  </tr>
		<tr>
		<td colspan="5"><b>* M=Mandatory R=Required O=Optional</b></td>
		</tr>
 </tbody>
</table>


##  Example Examination Findings Section ##

<script src="https://gist.github.com/IOPS-DEV/d39ad2e1297ea67df7488910d97d4a3b.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK3 FHIR Outpatient Letter does not currently support coded examination findings.







