---
title:  Individual Requirements Section
keywords:  messaging, sections
tags: [fhir,messaging,section]
sidebar: foundations_sidebar
permalink: explore_individual_reqs.html
summary: "Gives information about the Individual requirements section"
---

{% include custom/section.warnbanner.html %}

## Individual Requirements Section Content ##
The Individual requirements section carries information about the individual requirements of the patient. PRSB Elements should be formatted as subheadings in any HTML sent.

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
   <td>Individual requirements </td>
   <td>Individual requirements that a person has, e.g. communication, cultural, cognitive or mobility needs. </td>
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
   <td>Individual requirements</td>
   <td>Individual requirements that a person has. These may be communication, cultural, cognitive or mobility needs.</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>Information volunteered by the person or their representative or carer, or known about locally. Text or coded text (SNOMED CT), constrained as specified in SCCI1605.Accessible Information standard (accessible information - communications support, accessible information - requires communications professional, accessible information - requires specific contact method, accessible information - requires specific information format).

<b>Note: There is currently no support for this information to be coded in the FHIR Profiles and therefore this information should be sent as text only and this SNOMED CT information should seen as a place holder for future use.</b>
<ul>
<li>
Personal Preferences subset - https://dd4c.hscic.gov.uk/dd4c/publishedmetadatas/intid/225</li>
<li>Accessible information subsets</li>
<ul>
<li>https://dd4c.hscic.gov.uk/dd4c/publishedmetadatas/intid/657</li>
<li>https://dd4c.hscic.gov.uk/dd4c/publishedmetadatas/intid/660</li>
<li>https://dd4c.hscic.gov.uk/dd4c/publishedmetadatas/intid/658</li>
<li>https://dd4c.hscic.gov.uk/dd4c/publishedmetadatas/intid/659</li>
</ul>
<li>Mobility subsets</li>
<ul>
<li>https://dd4c.hscic.gov.uk/dd4c/publishedmetadatas/intid/762</li>
<li>https://dd4c.hscic.gov.uk/dd4c/publishedmetadatas/intid/181</li>
</ul>
<li>Cognition</li>
<ul>
<li>https://dd4c.hscic.gov.uk/dd4c/publishedmetadatas/intid/9</li>
</ul>
</ul>
</td>
  </tr>
 </tbody>
</table>

##  Example Individual Requirements Section ##

<script src="https://gist.github.com/IOPS-DEV/497e71d591b9041c318dc4c88517287b.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK3 FHIR Outpatient Letter does not currently support coded individual requirements information.







