---
title: Allergies and Adverse Reactions Section
keywords:  messaging, sections
tags: [fhir,messaging,section]
sidebar: foundations_sidebar
permalink: explore_allergies_and_adverse_reactions.html
summary: "Gives information about the Allergies and adverse reactions section"
---

{% include custom/section.warnbanner.html %}

## Allergies and Adverse Reactions Section Content##
The Allergies and adverse reactions section carries information about the patient's allergies and adverse reactions, items in bold are subheadings and should be formatted as such in any html sent:

- **Causative agent** - The agent such as food, drug or substances that has caused or may cause an allergy, intolerance or adverse reaction in this patient.</li>
- **Description of reaction** -	A description of the manifestation of the allergic or adverse reaction experienced by the patient. For example, skin rash.
-**Type of reaction** -	The type of reaction experienced by the patient (allergic, adverse, intolerance)
- **Severity** - A description of the severity of the reaction
- **Certainty** - A description of the certainty that the stated causative agent caused the allergic or adverse reaction.
- **Evidence** - Results of investigations that confirmed the certainty of the diagnosis. Examples might include results of skin prick allergy tests
- **Probability of recurrence** - Probability of the reaction (allergic, adverse, intolerant) occurring.
- **Date first experienced** - When the reaction was first experienced. May be a date or partial date (e.g. year) or text (e.g. during childhood)



##  Example Allergies and Adverse Reactions Sections ##

### Allergy to Penicillin ###

<script src="https://gist.github.com/IOPS-DEV/c02f9626ad71d2230cd51ded6d031bb2.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- List
- AllergyIntolerance
- Flag
 
See constructing coded clinical structures - [Allergy Lists](build_allergy_lists.html)









