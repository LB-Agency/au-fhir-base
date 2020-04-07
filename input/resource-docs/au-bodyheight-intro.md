**AU Body Height**  *[[FMM Level 2](guidance.html)]*

This profile defines a body height information structure for use in an Australian context that tightens the BodyHeightCode slice, aligning to the proposed [R4 Observation Body Height](http://build.fhir.org/bodyheight.html) profile.

As per the [R4 Vital Signs](http://build.fhir.org/observation-vitalsigns.html#vitals-table.html) guidance, a separate profile for Body Length is not supported. This observation may be supplemented with an additional coding element containing the LOINC code 8306-3 -*Body height - lying* (i.e., body length - typically used for infants).

Note: Known issues with vital signs and observation constraints should be considered when using this profile FHIR R4 has corrections that may be useful<sup>[1](http://hl7.org/fhir/R4/observation.html#invs)</sup><sup>[2](http://hl7.org/fhir/R4/vitalsigns.html#10.1.20.2.3)</sup>