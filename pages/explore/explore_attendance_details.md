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
The Attendance details section carries information about the patient's attendance at the Outpatient department. PRSB Elements should be formatted as subheadings in any HTML sent:

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
   <td>Attendance details</td>
   <td>The details of the patient contact.</td>
   <td>1 only</td>
   <td>M</td>
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
   <td>Date and time of contact</td>
   <td>Date and time of the appointment, contact or attendance.</td>
   <td>1 only</td>
   <td>M</td>
   <td>The date and time of appointment as recorded on the Patient Administration System (PAS) as text and carried in the <b>Encounter.period.start</b> and <b>Encounter.period.end</b>FHIR element.</td>
  </tr>
  <tr>
   <td>Contact type</td>
   <td>First contact, follow-up contact.</td>
   <td>0 to 1</td>
   <td>O</td>
   <td>Text. Contact type may come from those recorded on the local PAS.NHS Data dictionary First attendance. 
<ul>
<li>1<&nbsp>	First attendance face to face</li>
<li>2<&nbsp>	Follow-up attendance face to face</li>
<li>3<&nbsp>	First telephone or telemedicine consultation</li>
<li>4<&nbsp>	Follow-up telephone or telemedicine consultation</li>
</ul>
This should also be carried in the FHIR element <b>Encounter.type</b> and as this is an example ValueSet the <b>Encounter.type.Coding.system</b> should contain the value "https://www.datadictionary.nhs.uk".
</td>
  </tr>
  <tr> 
   <td>Consultation method</td>
   <td>CONSULTATION METHOD USED identifies the communication mechanism used to relay information between the CARE PROFESSIONAL and the PERSON who is the subject of the consultation, during the Outpatient encounter</td>
   <td>0 to 1</td>
   <td>R</td>
   <td>Text only, but may be derived from Consultation method from NHS Data Dictionary.
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
   <td>M</td>
 	<td>The name and identifier of the consultant from a recognised source such as the Spine Directory Service, or a local identifier. Any identifiers <b>MUST NOT</b> be carried as text. The following FHIR Elements <b>SHOULD</b> be populated in the Practitioner and PractitionerRole Resources: 
		<ul>
			<li><b>Encounter.participant.individual.<br/>Reference.Practitioner.identifier</b></li>
			<li><b>Encounter.participant.individual.<br/>Reference.Practitioner.name</b></li>
			<li><b>PractitionerRole.code</b></li>
			<li><b>PractitionerRole.identifier</b></li></ul></td>
  </tr>
  <tr>
   <td>Specialty</td>
   <td>Specialties designated by royal colleges and faculties. E.g. orthopaedics, renal medicine, endocrinology, etc</td>
   <td>0 to 1</td>
   <td>R</td>
<td>Text for either the main specialty of the responsible clinician (as held on the Spine Directory Service), or the department from which the patient is attending. The specialty <b>SHOULD</b> be populated in the <b>PractitionerRole.specialty</b> FHIR element. The profile is currently bound to the FHIR ValueSet <a href="http://hl7.org/fhir/stu3/valueset-c80-practice-codes.html">c80-practice-codes</a> as preferred. This is proposed to be replaced by NHS Data main specialty code and therfore the current guidance is to not use the preferred ValueSet but to replace it using a code from <a href="https://www.datadictionary.nhs.uk/data_dictionary/attributes/m/main_specialty_code_de.asp?shownav=1">MAIN SPECIALTY CODE</a>. The FHIR CodeSystem element should be populated with "https://www.datadictionary.nhs.uk". As an alternative this element may be populated with a SNOMED CT concept and the FHIR CodeSystem element populated with "http://snomed.info/sct". Note further guidance will be issues in a later release of the specification.</td>
  </tr>
  <tr>
   <td>Service</td>
   <td>Treatment functions or services. E.g. hand surgery, back surgery, hand clinic, TIA clinic, falls clinic, speech and language therapy, dialysis, family therapy, pre-admission assessment clinic, etc</td>
   <td>0 to 1</td>
   <td>R</td>
   <td>Text only.</td>
  </tr>
  <tr>
   <td>Seen by</td>
   <td>Doctor, nurse or other healthcare professional that sees the patient. Record the most senior member of staff present. Includes name, role, telephone number</td>
   <td>1 to many</td>
   <td>M</td>
   			<td>The name and identifier of the consultant from a recognised source such as the Spine Directory Service, or a local identifier. Any identifiers <b>MUST NOT</b> be carried as text. The following FHIR Elements <b>SHOULD</b> be populated in the Practitioner and PractitionerRole Resources: 
			<ul>
			<li><b>Encounter.participant.individual.<br/>Reference.Practitioner.identifier</b></li>
			<li><b>Encounter.participant.individual.<br/>Reference.Practitioner.name</b></li>
			<li><b>PractitionerRole.code</b></li>
			<li><b>PractitionerRole.identifier</b></li></ul></td>
  </tr>
  <tr>
   <td>Care professionals present</td>
   <td>The name, designation of the additional individuals or team members including consultant(s), nurse consultant(s), allied health professional(s), social worker(s)</td>
   <td>0 to many</td>
   <td>O</td>
   			<td>The name and identifier of the consultant from a recognised source such as the Spine Directory Service, or a local identifier. Any identifiers <b>MUST NOT</b> be carried as text. The following FHIR Elements <b>SHOULD</b> be populated in the Practitioner and PractitionerRole Resources: 
			<ul>
			<li><b>Encounter.participant.individual.<br/>Reference.Practitioner.identifier</b></li>
			<li><b>Encounter.participant.individual.<br/>Reference.Practitioner.name</b></li>
			<li><b>PractitionerRole.code</b></li>
			<li><b>PractitionerRole.identifier</b></li></ul></td>
  </tr>
  <tr>
   <td>Person accompanying patient</td>
   <td>Identify, where clinically relevant, others accompanying the patient, e.g. relative, friend, informal carer, advocate. If the patient was not present, was an authorised representative present? Includes: Name, Relationship, Role (patient advocate)</td>
   <td>0 to 1</td>
   <td>O</td>
   <td>Information provided by patient or person accompanying patient.Text and where possible the name and identifier of the consultant from a recognised source such as the Spine Directory Service, or a local identifier. Any identifiers <b>MUST NOT</b> be carried as text. The following FHIR Elements <b>SHOULD</b> be populated in the Practitioner and PractitionerRole Resources: 
			<ul>
			<li><b>Encounter.participant.individual.<br/>Reference.Practitioner.identifier</b></li>
			<li><b>Encounter.participant.individual.<br/>Reference.Practitioner.name</b></li>
			<li><b>PractitionerRole.code</b></li>
			<li><b>PractitionerRole.identifier</b></li></ul>
  </td>
  </tr>
  <tr>
   <td>Outcome of outpatient attendance</td>
   <td>This records the outcome of an Out-Patient Attendance</td>
   <td>0 to 1</td>
   <td>R</td>
   <td>Text only derived from the NHS Data DictionaryNational Codes:
<ul><li>1 - Discharged from CONSULTANT's care (last attendance)</li>
<li>2 - Another APPOINTMENT given</li>
<li>3 - APPOINTMENT to be made at a later date.</li></ul></td>
  </tr>
		<tr>
		<td colspan="5"><b>* M=Mandatory R=Required O=Optional</b></td>
		</tr>
 </tbody>
</table>



##  Example Attendance Details Section ##

<script src="https://gist.github.com/IOPS-DEV/ca6f27726a82f33981f972a17e6b2710.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK3 FHIR Outpatient Letter does not currently support coded Attendance details.








