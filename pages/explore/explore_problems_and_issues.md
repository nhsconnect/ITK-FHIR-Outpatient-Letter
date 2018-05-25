---
title: Problems and Issues Section
keywords:  messaging, sections
tags: [fhir,messaging,sections]
sidebar: foundations_sidebar
permalink: explore_problems_and_issues.html
summary: "Gives information about the Problems and issues section"
---

{% include custom/section.warnbanner.html %}

## Problems and Issues Section Content##
The Problems and issues section carries information about problems and issues. Elements should be formatted as sub headings in any HTML sent.

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
   <td>Problems and issues</td>
   <td>A summary of the problems that require investigation or treatment.</td>
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
   <td>Problems and issue</td>
   <td>Summary of problems that require investigation or treatment. This would include significant examination findings, symptoms and signs, which are likely to have relevance and are not a diagnosis.</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>Text. The problems and issues heading is for the clinician or healthcare professional's recording of medical problems and issues.</td>
  </tr>
 </tbody>
</table>


##  Example Problems and Issues Section ##

<script src="https://gist.github.com/IOPS-DEV/ede119d0b2d9782016b90466cadcabc7.js"></script>

## Coded Resources ##

- The ITK FHIR Outpatient Letter does not currently support a coded problems and issues.

 







