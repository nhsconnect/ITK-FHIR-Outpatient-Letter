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
The Allergies and adverse reactions section carries information about the patient's allergies and adverse reactions. Elements should be formatted as sub headings in any html sent.

<table class="tableizer-table">
 <thead>
  <tr class="tableizer-firstrow">
   <th>Section</th>
   <th>Description</th>
   <th>Cardinality</th>
   <th>MRO*</th>
   <th>Values</th>
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
   <td>Element</td>
   <td>Description</td>
   <td>Cardinality</td>
   <td>MRO*</td>
   <td>Values</td>
  </tr>
  <tr>
   <td>Causative agent</td>
   <td>The agent such as food, drug or substances that has caused or may cause an allergy, intolerance or adverse reaction in this patient. Or "No known drug allergies or adverse reactions" Or "Information not available"</td>
   <td>1 only</td>
   <td>mandatory</td>
   <td>"Choice of•  Text•  Coded text-</td>
  </tr>
  <tr>
   <td>      SNOMED CT] subset=Causative agent??? Plus text options ""No known drug allergies or adverse reactions"" and ""Information not available""Or alternatively one of the following statements:""No known drug allergies or adverse reactions"" Or ""Information not available"" (Comment coding for this should be reviewed as the GP2GP causative agent work reaches completion)"</td>
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
   <td>"C</td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>      hoice of</td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>        Text</td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>        Coded text -  constraint: SNOMED CT. Clinical finding. Any SNOMED CT term in the Clinical Finding hierarchy. Constraint binding: [SNOMED CT] subset=Clinical Finding"</td>
  </tr>
  <tr>
   <td>Severity</td>
   <td>A description of the severity of the reaction</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>"Coded text</td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>        </td>
  </tr>
  <tr>
   <td>          Mild [The reaction was mild.][SNOMED-CT::255604002] (Mild (qualifier value))</td>
  </tr>
  <tr>
   <td>          </td>
  </tr>
  <tr>
   <td>        </td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>        </td>
  </tr>
  <tr>
   <td>          Moderate [The reaction was moderate.][SNOMED-CT::6736007] (Moderate (severity modifier) (qualifier value))</td>
  </tr>
  <tr>
   <td>          </td>
  </tr>
  <tr>
   <td>        </td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>        </td>
  </tr>
  <tr>
   <td>          Severe [The reaction was severe.][SNOMED-CT::24484000] (Severe (severity modifier) (qualifier value))</td>
  </tr>
  <tr>
   <td>          </td>
  </tr>
  <tr>
   <td>        </td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>        </td>
  </tr>
  <tr>
   <td>          Life threatening [The reaction was life-threatening.][SNOMED-CT::442452003] (Life threatening severity (qualifier value))</td>
  </tr>
  <tr>
   <td>          </td>
  </tr>
  <tr>
   <td>        </td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>        </td>
  </tr>
  <tr>
   <td>          Fatal [The reaction was fatal.][SNOMED-CT::399166001] (Fatal (qualifier value))"</td>
  </tr>
  <tr>
   <td>Certainty</td>
   <td>A description of the certainty that the stated causative agent caused the allergic or adverse reaction.</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>"Coded text:</td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>        </td>
  </tr>
  <tr>
   <td>          Unlikely [The reaction is thought unlikely to have been caused by the agent.][SNOMED-CT::1491118016]</td>
  </tr>
  <tr>
   <td>          </td>
  </tr>
  <tr>
   <td>        </td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>        </td>
  </tr>
  <tr>
   <td>          Likely [The reaction is thought likely to have been caused by the agent.][SNOMED-CT::5961011]</td>
  </tr>
  <tr>
   <td>          </td>
  </tr>
  <tr>
   <td>        </td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>        </td>
  </tr>
  <tr>
   <td>          Certain [The agent is thought to be certain to have caused the reaction but this has not been confirmed by challenge testing.][SNOMED-CT::255545003] (Definite (qualifier value))t0018::</td>
  </tr>
  <tr>
   <td>          </td>
  </tr>
  <tr>
   <td>        </td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>        </td>
  </tr>
  <tr>
   <td>          Confirmed by challenge testing [The reaction to the agent has been confirmed by challenge testing or other concrete evidence.][SNOMED-CT::410605003] (Confirmed present (qualifier value))"</td>
  </tr>
  <tr>
   <td>Type of reaction</td>
   <td>The type of reaction experienced by the patient (allergic, adverse, intolerance)</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>"Coded text</td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>        Allergy</td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>        Intolerance</td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>        Adverse reaction</td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>    </td>
  </tr>
  <tr>
   <td>      </td>
  </tr>
  <tr>
   <td>        Not known"</td>
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



##  Example Allergies and Adverse Reactions Sections ##

### Allergy to Penicillin ###

<script src="https://gist.github.com/IOPS-DEV/c02f9626ad71d2230cd51ded6d031bb2.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- List
- AllergyIntolerance

 
See constructing coded clinical structures - [Allergy Lists](build_allergy_lists.html)









