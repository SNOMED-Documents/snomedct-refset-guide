# Appendix A: Overview of Reference Set Types

## Content Reference Sets

  

Table Appendix A:-1: Overview of reference set types and example use cases, as described in the international Release of SNOMED CT

  

**Reference Set Type**| **Description**| **Example Use Cases**  
---|---|---  
Simple reference set| Allows a set of components to be specified for inclusion or exclusion for a specified purpose | Constrain values available in clinical data entry templates. (E.g. define pick lists, constrain searches etc.)   
Specify values accepted for communication purposes in specific elements in a communication message   
Ordered reference set| Allows a collection of components to be defined with a specified given a priority ordering | Alternative navigation hierarchies. Specify a preferred order of concepts/descriptions in pick lists   
Attribute value reference set| Allows a value from a specified range to be associated with a component| This reference set type can be used for many different purposes that are related to both content and technical use cases. E.g. to specify why a concept or description has been inactivated   
Simple map reference set| Allows representation of simple maps between SNOMED CT concepts and values in other code systems. | Appropriate where there is a close "one-to-one" mapping between SNOMED CT concepts and coded values in another code system.   
Complex and Extended Map reference sets| Allows representation of simple complex maps between SNOMED CT concepts and values in other code systems | Enables representation of maps where each SNOMED CT concept may map to one or more codes in a target scheme, or where the correlation of each map should be specified   
Language reference set| Supports the representation of language and dialects preferences for the use of particular descriptions | Used to specify the acceptable and preferred terms for use within a particular country or region. Can also be used to represent preferences for use of descriptions in a more specific context such as a clinical specialty, organization or department   
Query specification reference set| Allows a serialized query to represent the membership of a subset of SNOMED CT components| Used to represent Intentional definitions of reference sets. Constrain values available in clinical data entry templates, as part of a terminology binding   
Annotation reference set| Allows text strings to be associated with components for any specified purpose| E.g. linking a SNOMED CT component to a url, e.g. for linking to a clinical guideline  
Association reference set| Represents a set of unordered associations of a particular type between components| Used to associate inactive concepts with active concepts that can serve as potential replacements for the inactivated concepts   
  
## Reference Sets for Technical Use

  

Table Appendix A:-1: Overview of reference set types and example use cases, as described in the international Release of SNOMED CT

  

**Reference Set Type**| **Description**| **Example Use Cases**  
---|---|---  
Module dependency reference set| Represents dependencies between different SNOMED CT release modules| The Module Dependency reference set is used to ensure that all dependencies are satisfied when importing data   
Description format reference set| Specifies the text format and maximum length of each supported description type| Specify new, localized description formats to be used in an Extension  
Reference set descriptor reference set| Represents the format of all reference sets included in a particular release | Specify new, customized reference set formats to be used in an Extension  
  
* * *
