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
The History section carries history related to the patient's previous care. Elements should be rendered as subheadings in any html sent.
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
   <td>History</td>
   <td>Information relating to the development of each presenting complaint, and the patient's relevant health history.</td>
   <td>0 to 1</td>
   <td>required</td>
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
   <td>Patient's reason for referral</td>
   <td>Patient stated reason for referral. This may include any discussions that took place, the level of shared decision making involved, information about patient's source of advice. This may be expressed on behalf of the patient, eg by parent or carer.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>The patient's reason for referral information will normally be provided during the outpatient consultation. Text</td>
  </tr>
  <tr>
   <td>Presenting complaints or issue</td>
   <td>The list and description of the health problems and issues experienced by the patient resulting in the attendance. This may include disease state, medical condition, response and reaction to therapies, eg blackout, dizziness, chest pain, follow-up from admission, falls, a specific procedure, investigation or treatment.</td>
   <td>0 to many</td>
   <td>required</td>
   <td>May be a SNOMED CT term or free text</td>
  </tr>
  <tr>
   <td>History of each presenting complaint or issue</td>
   <td>Information directly related to the development and characteristics of each presenting complaint (eg including travel history). Including if the information is given by the patient or their carer.</td>
   <td>0 to many</td>
   <td>optional</td>
   <td>This textual description may be provided by the referral document or during the consultation</td>
  </tr>
  <tr>
   <td>History since last contact</td>
   <td>History since last attendance, discharge from hospital, etc.</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>Free text and to include adherence to treatment plan, where appropriate</td>
  </tr>
  <tr>
   <td>Relevant past medical, surgical and mental health history</td>
   <td>The record of the person's significant medical, surgical and mental health history. Including relevant previous diagnoses, problems and issues, procedures, investigations, specific anaesthesia issues, etc (will include dental and obstetric history)</td>
   <td>0 to many</td>
   <td>optional</td>
   <td>Information relating to past medical, surgical and mental health history may be provided by the referral document or during the consultation. May be a SNOMED CT term or free text</td>
  </tr>
 </tbody>
</table>


##  Example History Section ##

<script src="https://gist.github.com/IOPS-DEV/dad7e1028c8a046c3dbe44d03ef6c6fb.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- [Condition](build_conditions.html)
- [Observation](build_observations.html)
- [Procedure](build_procedures.html)





