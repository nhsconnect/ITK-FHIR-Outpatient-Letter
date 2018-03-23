---
title: Medications and Medical Devices Section
keywords:  messaging, sections
tags: [fhir,messaging,section]
sidebar: foundations_sidebar
permalink: explore_medication.html
summary: "Gives information about the Medications and medical devices section"
---

{% include custom/section.warnbanner.html %}

## Medications and Medical Devices Section Content ##
The Medications and medical devices section carries information about the patient's medication. Elements should be formatted as subheadings in any html sent:

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
   <td>Medications and Medical Devices </td>
   <td>The details of and instructions for medications and medical equipment the patient is using.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td/>
  </tr>
  <tr>
   <th>Element</th>
   <th>Description</th>
   <th>Cardinality</th>
   <th>MRO*</th>
   <th>Values</th>
  </tr>
  <tr>
   <th>Medication item cluster</th>
   <th/>
   <th/>
   <th/>
   <th/>
  </tr>
  <tr>
   <td>Medication name</td>
   <td>May be generic name or brand name (as appropriate).Mandatory medication name coded using a SNOMED CT/dm+d term where possible, allowing plain text for historical/patient reported items , extemporaneous preparations or those not registered in dm+d.Comment: e.g."Citalopram tab 20mg", "Trimethoprim"</td>
   <td>1 only</td>
   <td>mandatory</td>
   <td>"Choice of Text or text derived from SNOMED CT -  constraint: MedicationName. Any AMP/VMP/VTM/AMPP/VMPP subsets from the dm+d terminology. NHS dm+d<ul>
     <li>AMP ::352201000001139 NHS dm+d</li>
     <li>AMPP ::352401000001135 NHS dm+d</li>
     <li>VMP ::352701000001133 NHS dm+d</li>
     <li>VMPP ::352301000001131 NHS dm+d</li>
     <li>VTM ::352601000001138. Constraint binding: [dm+d]subset=NHS_dm+d"</li>
    </ul>
   </td>
  </tr>
  <tr>
   <td>Form</td>
   <td>Form of the medicinal substance e.g capsules, tablets, liquid. Not normally required unless a specific form has been requested by the prescriber.Comment: e.g. "Modified Release  Capsules"</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>"Choice of Text or text derived from SNOMED CT - constraint: DrugDoseForm. SNOMED CT CfH DoseForm termset. Any descendant of 421967003 | drug dose form. Constraint binding: [SNOMED CT]subset=CfH DoseForm"</td>
  </tr>
  <tr>
   <td>Route</td>
   <td>Medication administration description (oral, IM, IV, etc.): may include method of administration, (e.g., by infusion, via nebuliser, via NG tube).Optional medication route, using SNOMED CT terms where possible. Not generally applicable to product-based medication. Should not be used to specify a specific administration site, for which a separate archetype is used e.g. The Route is 'intraocular' the  Site may be 'Left eye'.  Comment: e.g. "Oral", "Intraocular". Note that this element supports multiple Routes to allow a choice to be specified by the prescriber</td>
   <td>0 to many</td>
   <td>optional</td>
   <td>Text or text derived from SNOMED CT -  constraint: NHS e-prescribing route of administration subset ID: 413001000001136 Original Id : 30201000001137 This is an extract from the SUBSET -BiAnnual-Drug-15.0.1-20130401: SnomedCT_GB1000001_20130401/Subsets/EPrescribing/NHS e-Prescribing route of administration subset. Constraint binding: [SNOMED-CT]subset=NHS e-Prescribing route of administration subset</td>
  </tr>
  <tr>
   <td>Site</td>
   <td>The anatomical site at which the medication is to be administered.Comment: e.g. "Left eye"</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>Text or text derived from SNOMED CT -  constraint: SiteOfMedicationAdministration. Any valid site for the administration of a medication. Constraint binding: [SNOMED-CT]subset= SiteOfMedicationAdministration"</td>
  </tr>
  <tr>
   <td>Method</td>
   <td>The technique or method by which the medication is to be administered.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>Text</td>
  </tr>
  <tr>
   <td>Dose directions description</td>
   <td>A single plain text phrase describing the entire medication dosage and administration directions, including dose quantity and medication frequency.Comment: e.g. "I tablet at night" or "20mg at 10pm" This is the form of dosage direction text normally available from UK GP systems.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>Text</td>
  </tr>
  <tr>
   <td>Dose amount description </td>
   <td>A plain text description of medication single dose amount, as described in the AoMRC medication headings.Comment: e.g. "30 mg" or "2 tabs". UK Secondary care clinicians and systems normally minimally structure their dose directions, separating Dose amount and Dose timing (often referred to as Dose and Frequency). This format is not normally used in GP systems, which will always import Dose and Frequency descriptions concatenated into the single Dose directions description.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>Text</td>
  </tr>
  <tr>
   <td>Dose timing description</td>
   <td>A plain text description of medication dose frequency, as described in the AoMRC medication headings.Comment: e.g. "Twice a day", "At 8am 2pm and 10pm". UK Secondary care clinicians and systems normally minimally structure their dose directions, separating Dose amount and Dose timing (often referred to as Dose and Frequency). This format is not normally used in GP systems, which will always import Dose and Frequency descriptions concatenated into the single Dose directions description</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>Text</td>
  </tr>
  <tr>
   <td>Parsable dose directions ***</td>
   <td>A parsable 'dose syntax' which carries dose strength, dose timing, dose duration and maximum dose information.Comment: e.g. "20-30mg ^4/6h prn [180mg /24h]" = 20 to 30 mgs, up to 4-6 hourly as required. Maximum 180mg in 24 hours. The 'as required reason' e.g. 'for pain' should be carried in the Additional Instruction element. Note that this is generally a symptom and is not the same as the Indication which will usually describe a diagnosis or condition. Where supported, this would generally be used to exchange dosage information between systems, while Structured dose directions are likely to be used only within openEHR-based systems</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>Text*** Data items acting as placeholders for future 'advanced' structured dose syntax solution. In sufficient information to detail these further at present</td>
  </tr>
  <tr>
   <td>Structured dose direction cluster</td>
   <td>A structural representation of the elements carried by the dose syntax in 'Parsable doseStrength / timing' i.e. dose strength, dose timing, dose duration and maximum dose</td>
   <td>0 to many</td>
   <td>optional</td>
   <td>-</td>
  </tr>
  <tr>
   <td>Structured dose amount cluster ***</td>
   <td>A structural representation of dose amount.  Comment: e.g. 20mg or 2 tablets This element will generally only be used when persisting data within systems with 'Parsable dose directions' being used to exchange the same information between systems.</td>
   <td>-</td>
   <td>optional</td>
   <td>-*** Data items acting as placeholders for future 'advanced' structured dose syntax solution. In sufficient information to detail these further at present</td>
  </tr>
  <tr>
   <td>Structured dose timing cluster ***</td>
   <td>A slot containing a structural, computable representation of dose timing and maximum dose.Comment: This element will generally only be used when persisting data within systems with 'Parsable dose directions' being used to exchange the same information between systems.</td>
   <td>-</td>
   <td>optional</td>
   <td>-*** Data items acting as placeholders for future 'advanced' structured dose syntax solution. In sufficient information to detail these further at present</td>
  </tr>
  <tr>
   <td>Dose direction duration</td>
   <td>Recommendation of the time period for which the medication should be continued, including direction not to discontinue.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>"Choice of test of text derived from codes
 <ul>
     <li>Continue indefinitely [The medication should be continued indefinitely.]</li>
     <li>Do not discontinue [The medication should be continued indefinitely and the prescriber highly recommends that it should never be discontinued. This is an AoMRC Clinical Headings recommendation.]</li>
     <li>Stop when course complete. [The medication should be stopped when the currently prescribed course has been completed.]</li>
     <li>Duration: Allowed values: years, months, weeks, days, hours >=0 days"</li>
    </ul>
   </td>
  </tr>
  <tr>
   <td>Additional instruction </td>
   <td>Additional multiple dosage or administration instructions as plain text. This may include guidance to the prescriber, patient or person administering the medication. In some settings, specific Administration Instructions may be re-labelled as "Patient advice' or 'Dispensing Instruction' to capture these flavours of instruction.  Comment: e.g. "Omit  morning dose on day of procedure", "for pain or fever", "Dispense weekly".</td>
   <td>0 to many</td>
   <td>optional</td>
   <td>TextRuntime name constraint:
<ul>
     <li>Additional instruction [Additional multiple dosage or administration instructions as plain text. This may include guidance to the prescriber, patient or person administering the medication. In some settings, specific Administration Instructions may be re-labelled as "Patient advice' or 'Dispensing Instruction' to capture these flavours of instruction.]</li>
     <li>Dispensing instruction [Multiple plain text to record complex dispensing arrangements, particularly for Controlled Drug instalment dispensing. 'Dispensing instructions' may be used as a specific label to overwrite 'Additional instructions' to align with legacy GP system behaviour.]</li>
     <li>Patient advice [Multiple plain text instructions intended for patient or carer. 'Patient advice' may be used as a specific label to overwrite 'Additional instructions' to align with legacy GP system behaviour.]</li>
     <li>Monitoring [Special instructions related to monitoring of medication, such as lab tests.]"</li>
    </ul>
   </td>
  </tr>
  <tr>
   <td>Course details cluster</td>
   <td>Details of the overall course of medication.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>-</td>
  </tr>
  <tr>
   <td>Course status **</td>
   <td>The status of this prescription in an ambulatory (outpatient/GP/community) context</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>Choice of text derived from codes** Data item not relevant to Hospital to GP discharge summary
 <li>Active [This is an active medication.]</li>
    <li>Discontinued [This is a medication that has been issued. dispensed or administered but has now been discontinued.]</li>
    <li>Never active [A medication which was ordered or authorised but has been cancelled prior to being issued, dispensed or administered.]</li>
    <li>Completed [The medication course has been completed.]</li>
    <li>Obsolete [This medication order has been superseded by another.]"</li>
   </td>
  </tr>
  <tr>
   <td>Start date/time</td>
   <td>The date and/or time that the medication course should begin.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>Date/time</td>
  </tr>
  <tr>
   <td>End date/time</td>
   <td>The date and/or time that the medication course should finish.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>Date/time</td>
  </tr>
  <tr>
   <td>Indication</td>
   <td>Reason for medication being prescribed, where known.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>A free text or text derived from terms giving the clinical indication or reason for ordering the medication. Code derived terms are preferable.Comment: e.g. "Angina". The Indication generally describes a condition or diagnosis</td>
  </tr>
  <tr>
   <td>Link to indication record</td>
   <td>A link to the record which contains the Indication for this medication order.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>URL</td>
  </tr>
  <tr>
   <td>Comment/recommendation</td>
   <td>Suggestions about duration and/or review, ongoing monitoring requirements, advice on starting, discontinuing or changing medication.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>Free text. Additional comment or recommendation about the medication course e.g. 'Patient named supply', 'unlicensed medication', 'Foreign brand' or monitoring recommendations</td>
  </tr>
  <tr>
   <td>Medication change summary cluster</td>
   <td>Records the changes made to medication since admission</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td/>
  </tr>
  <tr>
   <td>Status</td>
   <td>The nature of any change made to the medication since admission.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>"Choice of text or text derived from codes
<ul>
     <li>Continued [Medicine present on both admission and discharge with no amendments.]</li>
     <li>Added [Medicine present on discharge but not on admission]</li>
     <li>Amended [Medicine present on both admission and discharge but with amendment(s) since admission.]"</li>
    </ul>
   </td>
  </tr>
  <tr>
   <td>Indication</td>
   <td>Reason for change in medication, eg sub-therapeutic dose, patient intolerant.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>Text</td>
  </tr>
  <tr>
   <td>Date of latest change</td>
   <td>The date of the latest change - addition, or amendment</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>Date / time</td>
  </tr>
  <tr>
   <td>Description of amendment</td>
   <td>Where a change is made to the medication ie one drug stopped and another started or eg dose, frequency or route is changed.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>Text</td>
  </tr>
  <tr>
   <td>Comment</td>
   <td>Any additional comment about the medication change</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>Text</td>
  </tr>
  <tr>
   <td>Total dose daily quantity cluster **</td>
   <td>The total daily dose of this medication. This is helpful for estimating optimal adherence to dosing guidance. It may be computed from product/dose strength and frequency or entered manually.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>** Data item not relevant to Hospital to GP discharge summary</td>
  </tr>
  <tr>
   <td>Medical devices entry</td>
   <td>Any therapeutic medical device of relevance that does not have representation in the NHS dictionary of medicines and medical devices (dm+d).</td>
   <td>0 to many</td>
   <td>optional</td>
   <td>Text</td>
  </tr>
  <tr>
   <td>Medication discontinued entry</td>
   <td/>
   <td/>
   <td/>
   <td/>
  </tr>
  <tr>
   <td>Name of discontinued medication</td>
   <td>The name of the medication or medical device being discontinued</td>
   <td>1 only</td>
   <td>mandatory</td>
   <td>Text</td>
  </tr>
  <tr>
   <td>Status</td>
   <td>The nature of any change made to the medication since admission.</td>
   <td>1 only</td>
   <td>mandatory</td>
   <td>Text</td>
  </tr>
  <tr>
   <td>Indication</td>
   <td>The clinical indication for any changes in medication status</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>Text</td>
  </tr>
  <tr>
   <td>Date of latest change</td>
   <td>The date of the discontinuation</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>Date / time</td>
  </tr>
  <tr>
   <td>Description of amendment</td>
   <td>A description of any amendment</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>Text</td>
  </tr>
  <tr>
   <td>Comment</td>
   <td>Any additional comment about the medication change.</td>
   <td>0 to 1</td>
   <td>optional</td>
   <td>Text</td>
  </tr>
 </tbody>
</table>




## Example Medications and Medical Devices Section ##

<script src="https://gist.github.com/IOPS-DEV/0a5596bdf4ab2c880eacb409e44c09df.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- List
- MedicationStatement
- Flag
 
See constructing coded clinical structures - [Medication Lists](build_medication_lists.html)











