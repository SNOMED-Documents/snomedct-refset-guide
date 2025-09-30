# Appendix B: Deprecated Reference Set Types

This section contains information about reference set types that are now deprecated and replaced by enhanced reference set. The fact that a referenced set type is deprecated does **not** imply that reference sets of that type cannot be used. However, it does indicate that there is another reference set type that more effectively meets the use case(s) for which these reference sets were originally designed.

## Ordered Reference Set

{% hint style="warning" %}
This reference set type has been deprecated in favour of two new reference set types. Please see following sections for introduction to the:

* [Ordered component reference set](5-reference-set-types.md#ordered-component-reference-set)
* [Ordered association reference set](5-reference-set-types.md#ordered-association-reference-set)
{% endhint %}

The design of the ordered reference set supports three overall purposes:

1. To specify a sequential order of a subset of components
2. To specify prioritized groups within a subset of components
3. To define alternative hierarchies of components

### Ordering <a href="#orderedreferenceset-ordering" id="orderedreferenceset-ordering"></a>

Ordered reference set can also be used to create a simple ordered list of components, i.e. a list that do not include any nesting, or groups. For ordered lists that do not require grouping or hierarchical arrangement the value of linkedToId should be the digit zero (0), as this attribute becomes irrelevant.

This type of ordered reference set can for example be used to prioritize the sort order of the descriptions with identical terms when they are displayed. It can also be used to specify the order of descriptions displayed in a simple pick list.

<figure><img src=".gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

<figure><img src="https://confluence.ihtsdotools.org/download/attachments/35985666/worddav1bc9228010e80acf97a985485c16361f.png?version=1&#x26;modificationDate=1482423992000&#x26;api=v2" alt=""><figcaption><p>Ordered reference set with no groups</p></figcaption></figure>

### Prioritization <a href="#orderedreferenceset-prioritizationprioritization" id="orderedreferenceset-prioritizationprioritization"></a>

Prioritization is similar to order but multiple components may have the same rank. In this case the value of the order attribute specify a priority order for a group of components.

<figure><img src=".gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

<figure><img src="https://confluence.ihtsdotools.org/download/attachments/35985666/image2016-7-21%208%3A55%3A31.png?version=1&#x26;modificationDate=1482423992000&#x26;api=v2" alt=""><figcaption><p>Ordered reference set with prioritized groups</p></figcaption></figure>

### Alternative hierarchy <a href="#orderedreferenceset-alternativehierarchy" id="orderedreferenceset-alternativehierarchy"></a>

The diagram below Illustrates how the three attributes referencedComponentId, order and linkedToId are used to create an alternative hierarchical order of some of the concepts from the subtype hierarchy.

<figure><img src="https://confluence.ihtsdotools.org/download/attachments/35985666/worddav607276daeb2cf6f6bb54a6e6e3c871b5.png?version=1&#x26;modificationDate=1482423992000&#x26;api=v2" alt=""><figcaption><p>Ordered reference set example.</p></figcaption></figure>

### Reference Set Specific Attributes <a href="#orderedreferenceset-referencesetspecificattributes" id="orderedreferenceset-referencesetspecificattributes"></a>

**Specific reference set attributes used to build an alternative hierarchical view of SNOMED CT**

<table><thead><tr><th width="242.5234375">Attribute</th><th>Description</th></tr></thead><tbody><tr><td><strong>referencedComponentId</strong></td><td>The identifier of a SNOMED CT component that is included in the ordered list of alternative hierarchy.</td></tr><tr><td><strong>order</strong></td><td>Specifies the sort order of the list. The list is ordered by applying an ascending sort of the order value.<br>The value of order =1 represents the highest priority. A value of '0' is not allowed. Duplicate values are permitted and the sort order between two members with the same order value is not defined.<br>If the linkedToId value is not 0, sorting occurs within subgroups that share the same linkedToId value.</td></tr><tr><td><strong>linkedToId</strong></td><td>The identifier of a SNOMED CT component that acts as a grouper or hierarchy node, collecting together a subgroup from within the list.<br><br>This field either enables reference set member linked into a number of subgroups. These subgroups can be nested allowing representation of alternative hierarchies.<br><br>To link members into a subgroup, all components in the same subgroup should reference the same component. This can either be a component that represents the name of that subgroup or the first member of the subgroup. In the latter case, the first row of each subgroup will contain the same identifier in referencedComponentId and linkedToId and with order =1.<br><br>To link a number of children concepts to a single parent concept, one member record should exist per child, with the referencedComponentId field referencing the parent and this field referencing the child concept. The order field is then used to order the children concepts under the parent concept.</td></tr></tbody></table>

## Annotation Reference Set

900000000000516008 <mark style="color:blue;">|</mark> Annotation type reference set<mark style="color:blue;">|</mark> allows String to be associated with components for any specified purpose. So, where the 900000000000521006 <mark style="color:blue;">|</mark> Association type reference set<mark style="color:blue;">|</mark> linked a SNOMED CT component to another SNOMED CT components, the 900000000000516008 <mark style="color:blue;">|</mark> Annotation type reference set<mark style="color:blue;">|</mark> allow a SNOMED CT component to be linked to a non-standardized string annotation.

<figure><img src=".gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

\\

### Reference Specific Attributes <a href="#annotationreferenceset-referencespecificattributes" id="annotationreferenceset-referencespecificattributes"></a>

Besides from the 4 identification and versioning attributes, the annotation reference set type has following attributes.

<table><thead><tr><th width="207.10546875">Field</th><th width="121.859375">Data type</th><th>Purpose</th></tr></thead><tbody><tr><td>referencedComponentId</td><td>SCTID</td><td>The identifier of the component to be annotated.</td></tr><tr><td>annotation</td><td>String</td><td>The text annotation to attach to the component identified by referencedComponentId.</td></tr></tbody></table>

{% hint style="warning" %}
See specification: [DEPRECATED: Annotation Reference Set](https://app.gitbook.com/s/irKbJsZG57nSWZA4GT0M/reference-set-release-file-specification/5.2-reference-set-types/5.2.1-content-reference-sets/5.2.1.6-deprecated-annotation-reference-set)
{% endhint %}

<a href="https://docs.google.com/forms/d/e/1FAIpQLScTmbZIf0UEQwYDkY27EEWBkaiYkHSbR0_9DmFrMLXoQLyL7Q/viewform?usp=pp_url&#x26;entry.1767247133=Refset+Guide&#x26;entry.670899847=Appendix%20B%3A%20Deprecated%20Reference%20Set%20Types" class="button primary">Provide Feedback</a>
