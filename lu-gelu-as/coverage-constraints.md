# Coverage Constraints

**Purpose**: Verify that the features provided in the dataset adhere to the constraints specified in the INSPIRE application schema related to the coverage feature types.

**Prerequisites**

**Test method**

The following checks are performed for every feature in the dataset.

* Check that the spatial object type CoverageByDomainAndRange is provided and it is a subtype of GridCoverage (coverage whose domain consists of a collection of grid points).
* ADD COVERAGE SPECIFIC CONSTRAINTS

**Reference(s)**: 

* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 4 (2)
* [TG DS-LU](./README.md#ref_TG_DS_LU) 5.3.1.1.4

**Test type**: Manual

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

