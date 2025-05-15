# 4.1. Reference Set Types and Descriptors

SNOMED International specifies a set of reference set types, which describes its own specific properties. This means that reference sets that are developed to conform to a specified pattern will have the same release file format as other reference sets of the same type. 

The pattern of a specific reference set type is described by a Descriptor Template. This means that the Descriptor Template is represented by a set of members of the [ 900000000000456007 | Reference set descriptor reference set (foundation metadata concept)|](http://snomed.info/id/900000000000456007 "900000000000456007 | Reference set descriptor reference set \(foundation metadata concept\) |") . 

All Descriptor Templates present in the international Release of SNOMED CT can be found in the reference set Descriptor. 

All reference sets that are released as part of the International Edition or from a National Release Center will have an associated Descriptor Template for the reference set. Where using a reference set for which a Descriptor Template has not been created, and additional information about the reference set is needed, the Descriptor Template of the closest ancestor of the concept describing the reference set that does have a Descriptor Template may be used. This means that a reference sets with no specified Descriptor Template inherits the Template from its supertype. 

An organization that releases reference sets should only release them without Descriptor Templates if the reference set follows a predefined pattern or if it is sure that its consumers do not require the information held within the Descriptor Template. You should note that Descriptor Templates are optional for other organizations, besides from SNOMED International, that create reference sets that do not follow a predefined pattern. However, we strongly recommend to specify the reference set descriptor template in the reference set Descriptor, to support automatic processing, validation and sharing of the reference sets.The diagram below illustrates the different reference set types and highlight some of the specific reference sets that are included in the International Edition of SNOMED CT. 

<figure><img src="../../images/35985483.png" alt="" title=""><figcaption><p>Figure 4.1-1: Reference set types and reference sets included in the International Edition of SNOMED CT</p></figcaption></figure>

  

  

  

  

  

