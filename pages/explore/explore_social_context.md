---
title: Social Context Section
keywords:  messaging, sections
tags: [fhir,messaging,section]
sidebar: foundations_sidebar
permalink: explore_social_context.html
summary: "Gives information about the Social context section"
---

{% include custom/section.warnbanner.html %}

## Social Context Section Content##
The Social context section carries information about the social context of the patient. Elements should be formatted as sub headings in any html sent.

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
   <td>Social context</td>
   <td>The social setting in which the patient lives, such as their household, occupational history, and lifestyle factors.</td>
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
   <td>Household composition</td>
   <td>E.g., lives alone, lives with family, lives with partner, etc. This may be free text.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>This is the record of the people living in the household with the patient (including where the patient lives alone) as given by the patient or their representative or carer. Free text.</td>
  </tr>
  <tr>
   <td>Occupational history</td>
   <td>The current and/or previous relevant occupation(s) of the patient/individual.</td>
   <td>0 to many</td>
   <td>optional</td>
   <td>This is a record of the patient's current or previous occupations as volunteered by the patient or their representative or carer. Text or coded text (SNOMED CT). 999001571000000109 | Occupation simple reference set (foundation metadata concept) |</td>
  </tr>
  <tr>
   <td>Educational history</td>
   <td>The current and/or previous relevant educational history of the patient/individual</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>This is a record of the patient's current or previous educational history as volunteered by the patient or their representative or carer. Text.</td>
  </tr>
  <tr>
   <td>Lifestyle</td>
   <td>The record of lifestyle choices made by the patient which are pertinent to his or her health and well-being, eg the record of the patient's physical activity level, pets, hobbies,  and sexual habits</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>This is a record of the patient's lifestyle choices which are pertinent to his or her health as volunteered by the patient. Text or coded text (SNOMED CT).</td>
  </tr>
  <tr>
   <td>Smoking</td>
   <td>Latest or current smoking observation.</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>This is a record of the patient's attest or current smoking observation. Text or coded text (SNOMED CT).Text. Please note a project led by University of Birmingham, QEHB and RCP is developing standards for recording of smoking in EPRs.</td>
  </tr>
  <tr>
   <td>Alcohol intake</td>
   <td>Latest or current alcohol consumption observation</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>This is a record of the patient's attest or current alcohol consumption. Text or coded text (SNOMED CT). Please note a project led by University of Birmingham, QEHB and RCP is developing standards for recording of alcohol intake in EPRs.</td>
  </tr>
  <tr>
   <td>Drug/substance use</td>
   <td>Latest or current drug/ substance use observation</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>This is a record of the patient's attest or current drug/ substance use observation. Text.</td>
  </tr>
  <tr>
   <td>Social circumstances</td>
   <td>The record of a patient's social background, network and personal circumstances, eg housing, religious, ethnic and spiritual needs, social concerns and whether the patient has dependents or is a carer. May include reference to safeguarding issues that are recorded elsewhere in the record.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>This is a record of the patient's social background, network and personal circumstances as volunteered by the patient or their representative or carer. Text.</td>
  </tr>
  <tr>
   <td>Services and care</td>
   <td>The description of services and care providing support for patient's health and social wellbeing.</td>
   <td>0 to many</td>
   <td>optional</td>
   <td>This is a description of services and care providing support for patient's health and social well-being, as volunteered by the patient or their representative or carer, or sourced through patient records. Text.</td>
  </tr>
 </tbody>
</table>



##  Example Social Context Section ##

<script src="https://gist.github.com/IOPS-DEV/73932c1d2ee99e5fd832bcbfa1922092.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- [Observation(Occupational history)](build_observations.html)





