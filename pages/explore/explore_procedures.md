---
title: Procedures Section
keywords:  messaging, sections
tags: [fhir,messaging,section]
sidebar: foundations_sidebar
permalink: explore_procedures.html
summary: "Gives information about the Procedures section"
---

{% include custom/section.warnbanner.html %}

## Procedures Section Content##
The Procedures section carries information about the procedures that have been performed on the patient, items in bold are subheadings and should be formatted as such in any html sent:

- **Procedure** - The therapeutic or diagnostic procedure performed.
- **Anatomical site** - The body site of the procedure
- **Laterality** - Laterality of the procedure
- **Complications related to procedure** - Details of any intra-operative complications encountered during the procedure, arising during the patient’s stay in the recovery unit or directly attributable to the procedure.
- **Specific anaesthesia issues** - Details of any adverse reaction to any anaesthetic agents including local anaesthesia.  Problematic intubation, transfusion reaction, etc.
- **Comment** - Any further textual comment to clarify such as statement that information is partial or incomplete.


##  Example Procedures Sections ##

<script src="https://gist.github.com/IOPS-DEV/9aac8ea1c4e276ff1316608ea53b0c8e.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- [Procedure](build_procedures.html)










