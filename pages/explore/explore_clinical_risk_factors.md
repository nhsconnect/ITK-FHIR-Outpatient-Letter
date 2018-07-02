---
title: 	Relevant Clinical Risk Factors Section
keywords:  messaging, sections
tags: [fhir,messaging,sections]
sidebar: foundations_sidebar
permalink: explore_clinical_risk_factors.html
summary: "Gives information about the Relevant clinical risk factors section"
---

{% include custom/section.warnbanner.html %}

## Relevant Clinical Risk Factors Section Content##
The Relevant clinical risk factors section carries information about relevant clinical risk factors for the patient. PRSB Elements should be formatted as subheadings in any HTML sent.

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
   <td>Relevant clinical risk factors</td>
   <td>Whether the patient is at high risk of clinical deterioration, any relevant clinical risk factors and risk mitigation plans.</td>
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
   <td>Relevant clinical risk factor</td>
   <td>Factors that have been shown to be associated with the development of a medical condition being considered as a diagnosis/differential diagnosis. Eg being overweight, smoker, no use of sun screen, enzyme deficiency.</td>
   <td>0 to many</td>
   <td>optional</td>
   <td>Coded (SNOMED CT) or text</td>
  </tr>
  <tr>
   <td>Clinical risk assessment</td>
   <td>Specific risk assessments required/undertaken.</td>
   <td>0 to many</td>
   <td>optional</td>
   <td>Text</td>
  </tr>
  <tr>
   <td>Risk mitigation</td>
   <td>Action taken to reduce the clinical risk and date actions.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>Free text.</td>
  </tr>
 </tbody>
</table>

##  Example Relevant Clinical Risk Factors Section ##

<script src="https://gist.github.com/IOPS-DEV/f6d8aa342d912ba92bd8097a6ac1c94e.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK3 FHIR Outpatient Letter does not currently support coded relevant clinical risk factors information.

 







