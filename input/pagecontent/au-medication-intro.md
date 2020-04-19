**AU Base Medication** *[[FMM Level 2](guidance.html)]*

This profile defines a medication structure including core localisation concepts for use in an Australian context. 


#### Medication Coding
Medication codings are used to define relevant drug/medication concepts. This includes coding as:
* PBS Item Code - Pharmaceutical Benefits Scheme coding, claiming context is not relevant as medicine coding.
* GTIN - Global Trade Item Number, physical product reference.
* AMT Code - Australian Medicines Terminology, national drug terminology.
* MIMS Package - commonly used medicine coding.


#### Extensions
Extensions used in this profile:
* Medication.code.coding: Medication Type [<sup>[1]</sup>](http://hl7.org.au/fhir/StructureDefinition/medication-type) - used to distinguish a level classification when the same coding system is used.
* Medication Brand Name [<sup>[1]</sup>](http://hl7.org.au/fhir/StructureDefinition/medication-brand-name) -  This text-only extension is supplied to support a brand name where no brand concept coding is available. Use code if a brand concept coding is available. 
* Medication Generic Drug Name [<sup>[1]</sup>](http://hl7.org.au/fhir/StructureDefinition/medication-generic-name) - This text-only extension is supplied to support a generic name where no generic concept coding is available. Use code if a generic concept coding is available.
* NOTE: if extensions Medication Brand Name or Medication Generic Drug Name are used then code must also be used. 


**Examples**

[Fluconazole Dose Based Medication](Medication-MedicationDoseBased.html)

[Paracetamol Generic Pack](Medication-GenericPack0.html)

[Nexium Hp7 Brand Pack](Medication-BrandedPack0.html)

[Nexium Hp7 Combination Package with Product Parts](Medication-CombinationPackage0.html)

[Clarithromycin 500mg Tablet Unbranded Product](Medication-UnbrandedProduct0.html)

[Esomeprazole 20mg Tablet Unbranded Product](Medication-UnbrandedProduct1.html)

[Amoxicillin 500mg Capsule Unbranded Product](Medication-UnbrandedProduct2.html)

[Norvasc 10 mg Tablet Brand Product with Batch Details](Medication-BrandProductwithBatchDetails0.html)


The following examples have been taken from the [National guidelines for on-screen display of clinical medicines information – January 2016](https://www.safetyandquality.gov.au/publications/national-guidelines-for-on-screen-display-of-clinical-medicines-information/) published by the Australian Commission on Safety and Quality in Health Care. Care has been taken with the clinical content in the structured data, and construction of narrative to be consistent with the guidelines:

[Single active ingredient product: pack-based](Medication-BrandedPackSingleActiveIngredient0.html)

[Two active ingredients product](Medication-TwoActiveIngredientsProduct0.html)

[Product with four or more active ingredients](Medication-FourOrMoreActiveIngredientsProduct0.html)
