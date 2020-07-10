# Constraints

**Purpose**: Verify that the features provided in the dataset adhere to the constraints specified in the INSPIRE application schema.

**Prerequisites**

**Test method**

The following checks are performed for every feature in the dataset.

* Check that at least one of the attributes legislationCitation, regulationText or planDocument is populated with a non-void value.

**Reference(s)**: 

* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 4 (2)
* [TG DS-LU](./README.md#ref_TG_DS_LU) 5.3.6.1

**Test type**: Automated

**Notes** 

Verify that the OCL constraints that are specified in the UML model of the application schema are met, i.e. validate features against the constraints. For unmet constraints report [constraintViolation](#constraintViolation).

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
constraintViolation <a name="constraintViolation"/>  |  XML document '$filename', $featureType '$gmlid': The constraint '$constraint' is violated.

## Contextual XPath references

The namespace prefixes used as described in [README](./README.md#namespaces).

Abbreviation                                               |  XPath expression                     |Multiplicity       |Voidable
---------------------------------------------------------- | ------------------------------------- | ------------------|----------
legislationCitation <a name="legislationCitation"></a> | //schema-element(plu:OfficialDocumentation)/plu:legislationCitation|0..1 |Yes
regulationText <a name="regulationText"></a> 	| //schema-element(plu:OfficialDocumentation)/plu:regulationText|0..1 |Yes
planDocument <a name="planDocument"></a> 	| //schema-element(plu:OfficialDocumentation)/plu:planDocument|0..1 |Yes
