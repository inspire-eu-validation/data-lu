# Constraints

**Purpose**: Verify that the features provided in the dataset adhere to the constraints specified in the INSPIRE application schema.

**Prerequisites**

**Test method**

The following checks are performed for every feature in the dataset.

* Check that the rangeSet values is of type CategoryOrNilReason.
"NOTE: Range is based on either HILUCS or on a specific land use classification sytem defined by the data provider"

* Check that the spatial object type CoverageByDomainAndRange is only of subtypes of GridCoverage.


**Reference(s)**: 

* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 4 (2)
* [TG DS-lu](./README.md#ref_TG_DS_LU) 5.4

**Test type**: Automated

**Notes** 

Verify that the OCL constraints that are specified in the UML model of the application schema are met, i.e. validate features against the constraints. For unmet constraints report [constraintViolation](#constraintViolation).

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
constraintViolation <a name="constraintViolation"/>  |  XML document '$filename', $featureType '$gmlid': The constraint '$constraint' is violated.

## Contextual XPath references

The namespace prefixes used as described in [README](./README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
legalBasis <a name="legalBasis"></a> 	| 	//schema-element(am:ManagementRestrictionOrRegulationZone)/am:legalBasis
LegislationCitation <a name="LegislationCitation"></a> 	| 	//schema-element(am:ManagementRestrictionOrRegulationZone)/am:legalBasis/base2:LegislationCitation

TABLE TO BE COMPLETED
