# 3.2.3.2. Specifying Queries for Retrieval and Analysis

Both extensionally and intensionally defined subsets of SNOMED CT components are useful for specifying clinical queries. For example, subsets of SNOMED CT concepts can be used to categorize patient data by testing for membership in a predefined subset, which is represented as a reference set. 

The [SNOMED CT Expression Constraint Language](http://snomed.org/ecl) (ECL) enables simple queries over SNOMED CT content to be expressed. While the language itself does not support querying over the full EHR content, the [ECL](http://snomed.org/ecl) could be embedded within record-based query languages (such as SQL) to represent the terminological aspects of these queries. 

Related to reference sets, the [ECL](http://snomed.org/ecl) includes the ability to refer to a set of concepts that are referenced by members of a reference set. Additionally, it includes a range of features, such as refinements, disjunction, and conjunction, which support specialized queries. The _memberOf_ function evaluates to the set of concepts that are referenced by the given reference set. For example, the following expression constraint is satisfied by the set of concepts which are members of [ 649999999104 | Example problem list simple reference set|](http://snomed.org/fictid#649999999104 "\(eg:649999999104\)  | Example problem list simple reference set |") :

  * memberOf  [ 649999999104 | Example problem list simple reference set|](http://snomed.org/fictid#649999999104 "\(eg:649999999104\)  | Example problem list simple reference set |")

The diagram below illustrate how reference sets can be for specifying queries.

<figure><img src="../../../../images/35985612.png" alt="" title=""><figcaption><p>Figure 3.2.3.2-1: Using reference sets for specifying queries</p></figcaption></figure>

