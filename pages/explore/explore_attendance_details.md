---
title: Attendance Details Section
keywords:  messaging, sections
tags: [fhir,messaging,sections]
sidebar: foundations_sidebar
permalink: explore_attendance_details.html
summary: "Gives information about the Attendance details section"
---

{% include custom/section.warnbanner.html %}

## Attendance Details Section Content##
The Attendance details section carries information about the patient's attendance at the outpatients department. Elements should be formatted as subheadings in any html sent:

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
   <td>Attendance details</td>
   <td>The details of the patient contact.</td>
   <td>1 only</td>
   <td>mandatory</td>
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
   <td>Date and time of contact</td>
   <td>Date and time of the appointment, contact or attendance.</td>
   <td>1 only</td>
   <td>mandatory</td>
   <td>The date as recorded on the PAS</td>
  </tr>
  <tr>
   <td>Contact type</td>
   <td>First contact, follow-up contact.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>Text. Contact type may come from those recorded on the local PAS.NHS Data dictionary First attendance
<ul>
<li>First attendance -  face-to-face</li>
<li>Follow-up attendance -  face-to-face</li>
<li>First telephone or telemedicine consultation</li>
<li>Follow-up telephone or telemedicine interview"</li>
</ul>
</td>
  </tr>
  <tr>
   <td>Consultation method</td>
   <td>CONSULTATION METHOD USED identifies the communication mechanism used to relay information between the CARE PROFESSIONAL and the PERSON who is the subject of the consultation, during the Outpatient encounter</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>Consultation method may come from those recorded on the local PAS. NHS Data Dictionary.
<ul>
<li>Face-to-face,</li>
<li>telephone,</li>
<li>tele medicine web camera,</li>
<li>talk type for a PERSON unable to speak</li>
</ul>
</td>
  </tr>
  <tr>
   <td>Responsible healthcare professional</td>
   <td>The name and designation of the consultant, nurse consultant, midwife, allied health professional who has overall responsibility for the patient (may not actually see the patient)</td>
   <td>1 only</td>
   <td>mandatory</td>
   <td>Text</td>
  </tr>
  <tr>
   <td>Specialty</td>
   <td>Specialties designated by royal colleges and faculties. Eg orthopaedics, renal medicine, endocrinology, etc</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>Codeable concept. Concept -  reference to a terminology or text.NHS data dictionary Main specialty codes</td>
  </tr>
  <tr>
   <td>Service</td>
   <td>Treatment functions or services. Eg hand surgery, back surgery, hand clinic, TIA clinic, falls clinic, speech and language therapy, dialysis, family therapy, pre-admission assessment clinic, etc</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>Codeable concept. Concept -  reference to a terminology or text.GPSoC contracts require metadata from Correspondence care settinghttps://dd4c.hscic.gov.uk/dd4c/publishedmetadatas/intid/58?size=10</td>
  </tr>
  <tr>
   <td>Seen by</td>
   <td>Doctor, nurse or other healthcare professional that sees the patient. Record the most senior member of staff present. Includes name, role, telephone number</td>
   <td>1 to many</td>
   <td>mandatory</td>
   <td>May be more than one where a joint clinic is held, eg there may be two consultants in a joint clinicMay be a SNOMED CT term 307839005 or free text</td>
  </tr>
  <tr>
   <td>Care professionals present</td>
   <td>The name, designation of the additional individuals or team members including consultant(s), nurse consultant(s), allied health professional(s), social worker(s)</td>
   <td>0 to many</td>
   <td>optional</td>
   <td>There may be more than one entry</td>
  </tr>
  <tr>
   <td>Person accompanying patient</td>
   <td>Identify, where clinically relevant, others accompanying the patient, eg relative, friend, informal carer, advocate. If the patient was not present, was an authorised representative present? Includes: Name, Relationship, Role (patient advocate)</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>Information provided by patient or person accompanying patient.Text</td>
  </tr>
  <tr>
   <td>Outcome of outpatient attendance</td>
   <td>This records the outcome of an Out-Patient Attendance</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>NHS Data DictionaryNational Codes:1 Discharged from CONSULTANT's care (last attendance)2 Another APPOINTMENT given3 APPOINTMENT to be made at a later date</td>
  </tr>
 </tbody>
</table>



##  Example Attendance Details Section ##

<script src="https://gist.github.com/IOPS-DEV/ca6f27726a82f33981f972a17e6b2710.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK FHIR Outpatient letter does not currently support coded Attendance details.








