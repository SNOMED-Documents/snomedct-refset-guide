# 3.2.1. Search and Data Entry

Many clinical applications include data entry interfaces controlled or assisted by protocols, templates or structured data entry forms. Each field on a data entry form may allow only a limited set of terms or concepts to be entered . The set of candidate [term](https://confluence.ihtsdotools.org/display/DOCRELFMT/term+\(field\)) or [concept](https://confluence.ihtsdotools.org/display/DOCGLOSS/concept) may range from very small (e.g. a set of priorities for a procedure) to very large (e.g. any general diagnosis). [Reference sets](https://confluence.ihtsdotools.org/display/DOCGLOSS/Reference+set) can be used to restrict the possible values that meet the requirements of a particular data entry protocol.

Examples of using reference sets to support search and data entry include:

* [5.2.1.1 Simple Reference Set](https://confluence.ihtsdotools.org/display/DOCRELFMT/5.2.1.1+Simple+Reference+Set) can be used to constrain searches or provide values for selection lists.
* [5.2.1.8 Ordered Reference Set](https://confluence.ihtsdotools.org/display/DOCRELFMT/5.2.1.8+Ordered+Reference+Set) can be used to prioritize search results or provide an alternative ordering of search results.
* [5.2.1.6 DEPRECATED: Annotation Reference Set](https://confluence.ihtsdotools.org/display/DOCRELFMT/5.2.1.6+DEPRECATED%3A+Annotation+Reference+Set) can be used to supplement search results or data entry options with additional textual or coded information, such as advice on intended usage.
* [5.9. Language Reference Set](https://github.com/IHTSDO/snomedct-refset-guide/blob/main/3%20requirements-and-use-cases/3.2%20use-cases/3.2.1%20search-and-data-entry/5.9.-Language-Reference-Set_35985689.html) can be used to ensure that the preferred descriptions, for a given dialect, care setting or clinical context, are displayed.

A [SNOMED CT enabled application](https://confluence.ihtsdotools.org/display/DOCGLOSS/Enabled+application) can use an appropriate [reference set](https://confluence.ihtsdotools.org/display/DOCGLOSS/reference+set) to display the valid data entry options and constrain text searches. For more detailed use case examples, please refer to the following sections:

* [3.2.1.1. Constrain Data Entry](https://github.com/IHTSDO/snomedct-refset-guide/blob/main/3%20requirements-and-use-cases/3.2%20use-cases/3.2.1%20search-and-data-entry/3.2.1.1.-Constrain-Data-Entry_35985564.html)
* [3.2.1.2. Constrain Searches](https://github.com/IHTSDO/snomedct-refset-guide/blob/main/3%20requirements-and-use-cases/3.2%20use-cases/3.2.1%20search-and-data-entry/3.2.1.2.-Constrain-Searches_35985569.html)
* [3.2.1.3. Exclude Content](https://github.com/IHTSDO/snomedct-refset-guide/blob/main/3%20requirements-and-use-cases/3.2%20use-cases/3.2.1%20search-and-data-entry/3.2.1.3.-Exclude-Content_35985586.html)
* [3.2.1.4. Order Items for Search and Data Entry](https://github.com/IHTSDO/snomedct-refset-guide/blob/main/3%20requirements-and-use-cases/3.2%20use-cases/3.2.1%20search-and-data-entry/3.2.1.4.-Order-Items-for-Search-and-Data-Entry_35985577.html)
* [3.2.1.5. Alternative Hierarchical View](https://github.com/IHTSDO/snomedct-refset-guide/blob/main/3%20requirements-and-use-cases/3.2%20use-cases/3.2.1%20search-and-data-entry/3.2.1.5.-Alternative-Hierarchical-View_35985573.html)
* [3.2.1.6. Use Case Specific Associations](https://github.com/IHTSDO/snomedct-refset-guide/blob/main/3%20requirements-and-use-cases/3.2%20use-cases/3.2.1%20search-and-data-entry/3.2.1.6.-Use-Case-Specific-Associations_35985582.html)
