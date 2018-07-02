---
title: Family History Section
keywords:  messaging, sections
tags: [fhir,messaging,sections]
sidebar: foundations_sidebar
permalink: explore_family_history.html
summary: "Gives information about the Family history section"
---

{% include custom/section.warnbanner.html %}

## Family History Section Content##
The Family history section carries details of any family history. PRSB Elements should be formatted as subheadings in any HTML sent.
 
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
   <td>Family history</td>
   <td>Information on illness in family relations relevant to the health or care of the patient.</td>
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
   <td>Family history</td>
   <td>The record of relevant illness in family relations deemed to be significant to the care or health of the patient, including mental illness and suicide, genetic information etc.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>The record of relevant illnesses in family relations as volunteered by the patient or their carer or representative. Text and/or coded text (SNOMED CT). 999000771000000106 | Family history simple reference set (foundation metadata concept) |</td>
  </tr>
 </tbody>
</table>

##  Example Family History Section ##

<script src="https://gist.github.com/IOPS-DEV/b279b3ea09bf124c357405345f27b28c.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- [FamilyMemberHistory](build_familymemberhistorys.html)






