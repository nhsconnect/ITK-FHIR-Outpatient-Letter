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
The Attendance details section carries information about the patient's attendance at the outpatients department.Items in bold are subheadings and should be formatted as such in any html sent:

- **Date of appointment/contact** - 	Date of the patient’s contact/appointment with the outpatient department.The date as recorded on the PAS
- **Contact type	First contact, follow-up contact** Contact type may come from those recorded on the local PAS.
- **Consultation method** - identifies the communication mechanism used to relay information between the care professional and the person who is the subject of the consultation, during the Outpatient encounter.	
- **Responsible healthcare professional** - The name and designation of the consultant, nurse consultant, midwife, allied health professional who has overall responsibility for the patient (may not actually see the patient).
- **Specialty**	- Specialties designated by royal colleges and faculties. Eg orthopaedics, renal medicine, endocrinology, etc.
- **Service** -	Treatment functions or services. Eg hand surgery, back surgery, hand clinic, TIA clinic, falls clinic, speech and language therapy, dialysis, family therapy, pre-admission assessment clinic, etc.	
- **Seen by** -	Doctor, nurse or other healthcare professional that sees the patient. Record the most senior member of staff present. Includes name, role, telephone number	
- **Care professionals present** - The name, designation of the additional individuals or team members including consultant(s), nurse consultant(s), allied health professional(s), social worker(s)
- **Person accompanying patient** -	Identify, where clinically relevant, others accompanying the patient, eg relative, friend, informal carer, advocate. If the patient was not present, was an authorised representative present? Includes: Name, Relationship, Role (patient advocate)
- **Outcome of outpatient attendance** - This records the outcome of an Out-Patient Attendance.


##  Example Attendance Details Section ##

<script src="https://gist.github.com/IOPS-DEV/1de586b28972e8d12a2c073646336708.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- [Encounter](workflow_encounter.html)







