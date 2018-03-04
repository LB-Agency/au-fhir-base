**AU Base Patient Profile** *[FMM Level [1](guidance.html)]*

This profile defines a patient administration details structure that includes core localisation concepts.

#### Identifiers
These definitions represent common data held in the Patient.identifier element.

* __Individual Healthcare Identifier - IHI__ 

[Namespace Description](http://ns.electronichealth.net.au/id/hi/ihi/1.0/index.html){:target="_blank"}

[METeOR Description](http://meteor.aihw.gov.au/content/index.phtml/itemId/432495){:target="_blank"}

The numerical identifier that uniquely identifies each individual in the Australian healthcare system.

The IHI identifier may also include extension properties IHI Status and IHI Record Status associated with the IHI value.

* __Medicare Number__ 

[Namespace Description](http://ns.electronichealth.net.au/id/medicare-number/index.html){:target="_blank"}

[METeOR Description](http://meteor.aihw.gov.au/content/index.phtml/itemId/270101){:target="_blank"}

Person identifier, allocated by the Health Insurance Commission to eligible persons under the Medicare scheme, that appears on a Medicare card.

The Medicare card number should only be collected from persons eligible to receive health services that are
to be funded by the Commonwealth government. The number should be reported to the appropriate government 
agency to reconcile payment for the service provided. The data should not be used by private sector 
organisations for any other purpose unless specifically authorised by law. For example, data linkage 
should not be carried out unless specifically authorised by law.

Medicare number may also include an expiry date associated with the number.

* __DVA (Department of Veterans' Affairs) Number__ 

[Namespace Description](http://ns.electronichealth.net.au/id/dva/index.html){:target="_blank"}

[METeOR Description](http://meteor.aihw.gov.au/content/index.phtml/itemId/339127){:target="_blank"}

The data should not be used by private sector organisations for any purpose unless specifically authorised by law. For example, 
private sector organisations should not use the DVA file number for data linking unless specifically authorised by relevant 
privacy legislation.

DVA number may also include details of the specific card colour associated with the number.

* __Health Care Card Number__ 
* __Pensioner Concession Card Number__ 
* __Commonwealth Seniors Health Card Number__ 

[Namespace Description](http://ns.electronichealth.net.au/id/centrelink-customer-reference-number/index.html){:target="_blank"}

[METeOR CRN Description](http://meteor.aihw.gov.au/content/index.phtml/itemId/270098){:target="_blank"}

All of the above mentioned cards use Centerlink Customer Reference Number.

A personal identifier assigned by Centrelink for the purposes of identifying people (and organisations) eligible for specific 
services, including some public health care services, such as oral health services.

The CRN should only be collected from persons eligible to receive health services that are to be funded by Centrelink. The 
number may be reported to a Centrelink agency to reconcile payment for the service provided. The data should not be used by
private sector organisations for any purpose unless specifically authorised by law. For example, data linkage should not be
carried out unless specifically authorised by law.

#### Extensions
Definitions here describe extensions to the Patient resource.

* __Indigenous Status__  

[METeOR Description](http://meteor.aihw.gov.au/content/index.phtml/itemId/602543){:target="_blank"}

This extension is added to hold the administrative indigenous status of an individual. The Commonwealth defintion
of indigenous status is "An Aboriginal or Torres Strait Islander is a person of Aboriginal or Torres Strait Islander 
descent who identifies as an Aboriginal or Torres Strait Islander and is accepted as such by the community in which
he or she lives"

Indigenous status is defined as a coded concept associated with the patient.

* __Close the Gap Registration__ 

[As per CTG indicator](http://meteor.aihw.gov.au/content/index.phtml/itemId/603679){:target="_blank"}

An extension to hold the indication of registration to the Close the Gap co-payment scheme status for the patient.  The CTG PBS Co-payment 
Measure improves access to PBS medicines for eligible Aboriginal and Torres Strait Islanders living with, or at risk of, 
chronic disease.

* __Birth Time__

[Standard STU3 extension](http://hl7.org/fhir/STU3/extension-patient-birthtime.html)

An extension to record the time of day that the Patient was born. This includes the date to ensure that the timezone information can be communicated effectively.

**Examples**

[Patient with IHI, Medicare Number, and Health Care Card](Patient-example0.html)

[Patient with IHI and DVA Number](Patient-example1.html)
