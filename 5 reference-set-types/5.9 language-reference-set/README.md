# 5.9. Language Reference Set

Language reference sets are used to specify the acceptability and preference for using a particular description in a specific language, dialect or clinical context. To understand the importance of Language reference sets it is necessary to be aware of the characteristics of SNOMED CT Descriptions and their representation.

## Descriptions and Language Reference Set

SNOMED CT contains descriptions and each description contains both a human-readable term and some information about the term. A description is used to give meaning to a concept and provide well-understood and standard ways of referring to a concept. So, each description is associated with a specific concept, but each concept is associated to several descriptions. Additionally, the descriptions are specific to a language or dialect.

All Descriptions are of a specific type and the most common description types are the [Fully Specified Name](https://confluence.ihtsdotools.org/display/DOCGLOSS/Fully+Specified+Name "Glossary link: Fully Specified Name")and [Synonym](https://confluence.ihtsdotools.org/display/DOCGLOSS/Synonym "Glossary link: Synonym"). The Description file holds descriptions that describe SNOMED CT concepts. The description file is released with the International Edition of SNOMED CT. National or Affiliate Editions may develop their own description file, e.g. to represent description in their own language and/or dialects.

The Language reference set is essential to enable the preferred terms to be identified for each concept. [Language reference sets](5.9.-Language-Reference-Set_35985689.html) refers to Descriptions that is used in a particular language or dialect. For each Description referenced in the language reference set a value for the acceptability of the term associated with that Description is assigned. The values for the Acceptability attribute is represented by descendants of the concept [ 900000000000511003 | Acceptability|](http://snomed.info/id/900000000000511003 "900000000000511003 | Acceptability |") , which is placed in the foundation metadata subhierarchy of SNOMED CT.

<figure><img src="plugins/servlet/confluence/placeholder/unknown-macro" alt="" title=""><figcaption><p>Value| Description</p></figcaption></figure>|---  
**900000000000548007 | Preferred (foundation metadata concept) |**|  The term associated with this description is the preferred description, of the specified Description.typeId, for the associated concept, in the language or dialect represented by this reference set.  
If the Description.typeId is synonym, this description is the preferred term.  
If the Description.typeId is fully specified name this description is the preferred fully specified name.  
For each concept there should be exactly one preferred description of each Description.typeId in each language reference set.  
**900000000000549004 | Acceptable (foundation metadata concept) |**|  The term associated with this description is acceptable for use in language or dialect represented by this reference set.  
  
  

The following diagram shows an example of the description file included in the International Release and the US Language reference set, which is also distributed with the International Release of SNOMED CT. The language reference set states the acceptability of the descriptions, i.e. whether they are preferred or synonym. For each concept there may be any number of acceptable descriptions of each description type in each language reference set. The diagram below shows how the description file holds information about the description type, and the language reference set specify the acceptability of the descriptions.

  

<figure><img src="../../images/35985696.png" alt="" title=""></figure>

<figure><img src="plugins/servlet/confluence/placeholder/unknown-macro" alt="" title=""><figcaption><p>Even though a concept has several descriptions of the type [ 900000000000013009 | Synonym (core metadata concept)|](http://snomed.info/id/900000000000013009 "900000000000013009 | Synonym \(core metadata concept\) |") related to it, the [language reference set](5.9.-Language-Reference-Set<em>35985689.html) allows automatic identification of the [preferred term](https://confluence.ihtsdotools.org/display/DOCGLOSS/preferred+term "Glossary link: preferred term"). The language reference set does not contain any terms, as these are represented in the description file. Hence, it refers to descriptions by referencing the [descriptionId](https://confluence.ihtsdotools.org/display/DOCGLOSS/description+identifier), and the description release file is therefore a prerequisite for retrieving the actual term when applying the [language reference set](5.9.-Language-Reference-Set</em>35985689.html) .</p></figcaption></figure>

  

  

<figure><img src="plugins/servlet/confluence/placeholder/unknown-macro" alt="" title=""><figcaption><p>Field| Data type| Purpose</p></figcaption></figure>|---|---  
[referencedComponentId](https://confluence.ihtsdotools.org/display/DOCRELFMT/referencedComponentId+\(field\) "Reference term: referencedComponentId \(field\)")| [SCTID](https://confluence.ihtsdotools.org/display/DOCRELFMT/6.1+SCTID+Data+Type)| The identifier of a [description](https://confluence.ihtsdotools.org/display/DOCGLOSS/description "Glossary link: description") included in the [language reference set](https://confluence.ihtsdotools.org/display/DOCRELFMT/5.2.2.1+Language+Reference+Set).  
[acceptabilityId](https://confluence.ihtsdotools.org/display/DOCRELFMT/acceptabilityId+\(field\) "Reference term: acceptabilityId \(field\)")| [SCTID](https://confluence.ihtsdotools.org/display/DOCRELFMT/6.1+SCTID+Data+Type)| A[subtype](https://confluence.ihtsdotools.org/display/DOCGLOSS/subtype "Glossary link: subtype")of [ 900000000000511003 | Acceptability|](http://snomed.info/id/900000000000511003 "900000000000511003 | Acceptability |") indicating whether the[description](https://confluence.ihtsdotools.org/display/DOCGLOSS/description "Glossary link: description")is acceptable or preferred for use in the specified[language](https://confluence.ihtsdotools.org/display/DOCGLOSS/language "Glossary link: language")or[dialect](https://confluence.ihtsdotools.org/display/DOCGLOSS/dialect "Glossary link: dialect").  
  
  

