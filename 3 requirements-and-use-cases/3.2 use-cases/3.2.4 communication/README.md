# 3.2.4 communication

## 3.2.4. Communication

Messages and communication services are a means of exchanging data and thus enable effective and efficient communication among healthcare professionals and between patients and providers. SNOMED CT is important for communication because it serves as a semantic foundation for the meaning expressed in a message. Hence, SNOMED CT can ensure consistent and accurate representation of the information communicated, and support correct interpretation of the clinical information within a message.

Communicating clinical data through messages support a range of purposes, including:

* Delivering accurate, accessible, and actionable health information that is targeted or tailored.
* Facilitating the meaningful use and exchange of health information among healthcare professionals.
* Supporting shared decision-making between patients and providers.
* Providing personalized self-management tools and resources.
* Building social support networks.
* Increasing health literacy skills.

## Use of SNOMED CT in Messages

Healthcare messages include fields that can be populated with codes from clinical coding schemes. [SNOMED CT](https://confluence.ihtsdotools.org/display/DOCGLOSS/SNOMED) provides [concept identifiers](https://confluence.ihtsdotools.org/display/DOCGLOSS/concept+identifier) as a means of encoding [concepts](https://confluence.ihtsdotools.org/display/DOCGLOSS/concept). These [concept identifiers](https://confluence.ihtsdotools.org/display/DOCGLOSS/concept+identifier) are suitable for use in appropriate fields of many clinical messages.

Implementations of clinical messaging typically constrain the range of values that can be applied to particular fields several reasons for this are listed in the following table.

Table 3.2.4-1: Reasons for constraining the content of fields in clinical messages

| Reason                                                                                   | Example                                                                                                                                                                                                                                                                                                                   |
| ---------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| To ensure that the information encoded is meaningful as a value for the specified field. | A field that is intended to describe the nature of investigation may contain a code that means "Serum glucose measurement" but should not contain a code that means "Hypoglycemia."                                                                                                                                       |
| To ensure that receiving application is able to process the message.                     | A locally added code value may be valid in a particular application but should not be used if the receiving application needs to retrieve, process or analyze the coded part of the message.                                                                                                                              |
| To ensure adequate detail and specificity.                                               | A field used to report an operative procedure could contain a code for "Abdominal procedure." However, this would not be adequate to meet the business purpose served by a message.                                                                                                                                       |
| To avoid unnecessary detail or diversity.                                                | A biochemical investigation could be reported using a code that represents various detailed aspects of the method used to perform the investigation. Such details may be unnecessary to a clinician and may complicate the analysis, charting and graphing of a series of results reported at different levels of detail. |

For a more detailed use case example, please refer to the following section:

* [3.2.4.1. Constraining the Coded Content of Messages](https://github.com/IHTSDO/snomedct-refset-guide/blob/main/3%20requirements-and-use-cases/3.2%20use-cases/3.2.4%20communication/3.2.4.1.-Constraining-the-Coded-Content-of-Messages_35985553.html)
