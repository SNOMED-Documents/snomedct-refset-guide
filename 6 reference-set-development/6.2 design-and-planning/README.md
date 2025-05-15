# 6.2. Design and Planning

Careful planning in the initial stage is crucial for successful completion of the reference set development and onwards use of the reference set. Following considerations should be included in any reference set development process. 

Table 6.2-1: Considerations important when designing the reference set and planning the development process

**Topic**| **Description**  
---|---  
Resources| Determine the resources available for developing and maintenance of the reference set.   
Dependencies| Dependencies of the reference set

  * What module and release of SNOMED CT is the reference set dependent on?
  * What other terminology and/or software artefact should the reference set function with? (see section on [6.2.2. Reference Sets and Information Models](6.2.2.-Reference-Sets-and-Information-Models_35985720.html)) 

  
Reference set type| What type of reference set is required?

  * Is one of the existing reference set patterns sufficient?
  * Should a customized reference set be specified, and if so what additional attributes should be included? 

  
People| Developing a new reference set requires a broad skillset, so it should be determined who will develop the reference set. Each of the steps related to developing reference sets can involve a range of people in different roles, a number of interdependent activities and a suite of related documents and artifacts. It is important to understand the characteristics of the people involved and their roles across the stages in the reference set lifecycle. 

  * Some of the important skills required when developing reference sets include:
    * clinical insight. To know what content is relevant for the specific purpose.
    * sufficient knowledge on SNOMED CT. To support correct use of SNOMED CT, for example selection of appropriate concepts or defining the correct query. 
    * knowledge about the technical environment where the subset is going to function. In order to ensure an appropriate representation of the subset to be integrated in an IT-system. 

  
Development approach and methods| What approach should be taken to develop the reference set?

  * Does any existing reference set meet the requirements for this new reference set or is there a need to build a new reference set from scratch? (see section on [6.2.1. Exploring and Evaluating Reference Sets](6.2.1.-Exploring-and-Evaluating-Reference-Sets_35985715.html)) 

  
Tools| What tools should be used to support reference set development, distribution and maintenance process?   
There will be a suite of tools provided which can support the creation and management of reference sets, including tools for: 

  * Selection of reference set members, or definition of the query needed to retrieve reference members. Such tool will typically allow collaborative approaches to be pursued. 
  * Support review by subject matter experts and others involved with creation and quality assurance 
  * Managing requests for change through a reporting mechanism that will allow potential changes to the reference set to be identified. 
  * Updating the reference set, e.g. when changes has been requested, or when new releases of the Editions on which the reference set is dependent upon is freed. 
    * SNOMED International provides a range of services and tools to support working with SNOMED CT, and the suite of services continue to grow. Specifically, the SNOMED International reference set management tool, which is useful the creation and management of both intensionally and extensionally defined subsets. 

  
Timeline| Determine when the reference set should be ready for routine use, i.e. schedule deadlines for the difference phases of the development process.   
Quality assurance| What level of quality is required for the reference set? E.g. is the reference set used to represent safety critical information for patients, or is the reference set used to form broader categories of patient groups. It should be determined how the required level of quality is obtained and ensured throughout the development process.   
Distribution| How will the reference set be distributed? Answering this question will depend very much on who the authors of the reference set is and where the reference set going to be used. If the reference set is used as a national reference set, i.e. a reference set which is used across a range of hospitals or organizations, distribution is likely to be done via a central service. Locally defined reference sets, e.g. used as part of configuring an EHR is likely to be managed and distributed from a local terminology storage environment and integrated directly to the system.   
Integration| How, who and when to integrate the reference set into the environment where it is going to function? Decide on an approach to integration and determine what bindings and/or integration tasks to be performed.   
Maintenance| Will new versions of the reference set be integrated regularly or as in integrated part of a greater maintenance process together with other software/terminology artefacts? 
