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
The Allergies and adverse reactions section carries information about the patient's allergies and adverse reactions. Elements should be formatted as subheadings in any HTML sent.

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
   <td>Allergies and adverse reactions</td>
   <td>The details of any known allergies, intolerances or adverse reactions.</td>
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
   <td>Causative agent</td>
   <td>The agent such as food, drug or substances that has caused or may cause an allergy, intolerance or adverse reaction in this patient. Or "No known drug allergies or adverse reactions" Or "Information not available"</td>
   <td>1 only</td>
   <td>mandatory</td>
   <td>Choice of text or text derived from SNOMED CT subset=Causative agent??? Plus text options "No known drug allergies or adverse reactions" and "Information not available"Or alternatively one of the following statements:"No known drug allergies or adverse reactions" Or "Information not available" (Comment coding for this should be reviewed as the GP2GP causative agent work reaches completion)"</td>
  </tr>
  <tr>
   <td>Reaction details cluster</td>
   <td>&nbsp;</td>
   <td>&nbsp;</td>
   <td>&nbsp;</td>
   <td>&nbsp;</td>
  </tr>
  <tr>
   <td>Description of reaction</td>
   <td>A description of the manifestation of the allergic or adverse reaction experienced by the patient. For example, skin rash.  Comment: this is Reaction in Scottish and English GP2GP models.</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>Choice of text or text derived from SNOMED CT - constraint: SNOMED CT. Clinical finding. Any SNOMED CT term in the Clinical Finding hierarchy. Constraint binding: [SNOMED CT] subset=Clinical Finding</td>
  </tr>
  <tr>
   <td>Severity</td>
   <td>A description of the severity of the reaction</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>Coded text 
<ul>
     <li>Mild - The reaction was mild.[SNOMED-CT::255604002] (Mild (qualifier value)</li>
     <li>Moderate - The reaction was moderate.[SNOMED-CT::6736007] (Moderate (severity modifier) (qualifier value)</li>
     <li>Severe - The reaction was severe.[SNOMED-CT::24484000] (Severe (severity modifier) (qualifier value)</li>
     <li>Life threatening -  The reaction was life-threatening.[SNOMED-CT::442452003] (Life threatening severity (qualifier value)</li>
     <li>Fatal - The reaction was fatal.[SNOMED-CT::399166001] (Fatal (qualifier value))</li>
    </ul>
   </td>
  </tr>
  <tr>
   <td>Certainty</td>
   <td>A description of the certainty that the stated causative agent caused the allergic or adverse reaction.</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>Text derived from SNOMED CT
<ul>
     <li>Unlikely - The reaction is thought unlikely to have been caused by the agent.[SNOMED-CT::1491118016]</li>
     <li>Likely - The reaction is thought likely to have been caused by the agent.[SNOMED-CT::5961011]</li>
     <li>Certain - The agent is thought to be certain to have caused the reaction but this has not been confirmed by challenge testing.[SNOMED-CT::255545003] (Definite (qualifier value))t0018::</li>
     <li>Confirmed by challenge testing - The reaction to the agent has been confirmed by challenge testing or other concrete evidence.][SNOMED-CT::410605003] (Confirmed present (qualifier value))"</li>
    </ul>
   </td>
  </tr>
  <tr>
   <td>Type of reaction</td>
   <td>The type of reaction experienced by the patient (allergic, adverse, intolerance)</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>Text derived from codes
<ul>
     <li>Allergy</li>
     <li>Intolerance</li>
     <li>Adverse reaction</li>
     <li>Not known</li>
    </ul>
   </td>
  </tr>
  <tr>
   <td>Evidence</td>
   <td>Results of investigations that confirmed the certainty of the diagnosis. Examples might include results of skin prick allergy tests</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>Text</td>
  </tr>
  <tr>
   <td>Probability of recurrence</td>
   <td>Probability of the reaction (allergic, adverse, intolerant) occurring</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>Text</td>
  </tr>
  <tr>
   <td>Date first experienced</td>
   <td>When the reaction was first experienced. May be a date or partial date (e.g. year) or text (e.g. during childhood)</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>Date/time</td>
  </tr>
 </tbody>
</table>

## How to Represent "No Known Allergies" ## 
When there is a positive statement that the patient has "No Known Allergies" then no coded structure is sent and the section is sent with a text string within the narrative. When the text string is derived from coded data it must match the text of the code: for example 716186003 "No known allergy"

##  Example Allergies and Adverse Reactions Sections ##

### Allergy to Penicillin ###

<script src="https://gist.github.com/IOPS-DEV/c02f9626ad71d2230cd51ded6d031bb2.js"></script>

### "No known allergy" ###

<script src="https://gist.github.com/IOPS-DEV/3f77d2ebcfcdf305a640484fb445cc1a.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- List
- AllergyIntolerance

 
See constructing coded clinical structures - [Allergy Lists](build_allergy_lists.html)









