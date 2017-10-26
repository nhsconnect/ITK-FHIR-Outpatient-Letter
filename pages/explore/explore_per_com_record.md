---
title: Person Completing Record Section
keywords:  messaging, sections
tags: [fhir,messaging,sections]
sidebar: foundations_sidebar
permalink: explore_per_com_record.html
summary: "Gives information about the Person completing record section"
---

{% include custom/section.warnbanner.html %}

## Person Completing Record Section Content##
The Person completing record section carries information about the person who completed the record. Items in bold are subheadings and should be formatted as such in any html sent:

- **Name** - The name of the person completing the record, preferably in a structured format.
- **Role**- The role the person is playing within the organisation at the time record was updated.
- **Grade** - The grade of the person completing the record
- **Specialty** -The main specialty of the person completing the record.
- **Professional identifier** - Professional identifier for the person completing the record e.g., GMC number, HCPC number etc or the personal identifier used by the local organisation.
- **Date and time completed** -	The date and time the record was updated.
- **Contact details** -	Contact details of the person completing the record. For example a phone number, email address. Contact details are used to resolve queries about the record entry.



## Example Person Completing Record Section ##

<script src="https://gist.github.com/IOPS-DEV/4eceababbca389067cde4aefd2d61cde.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK FHIR Outpatient letter does not currently support coded Person completing record information.






