# Coverage Constraints

**Purpose**: Verify that the features provided in the dataset adhere to the constraints specified in the INSPIRE application schema related to the coverage feature types.

**Prerequisites**

**Test method**

The following checks are performed for every feature in the dataset.

* Check that the spatial object type CoverageByDomainAndRange is provided and it is a subtype of GridCoverage (coverage whose domain consists of a collection of grid points). To fullfill this constraint verify that the following contraints defined by "INSPIRE Data Specifications – Base Models – Coverage Types" are met:
  * gridFunctionRequiresGridDomain: The grid function shall only be valid for domains that are grids (OCL: inv: coverageFunction.gridFunction.notEmpty() implies domainSet.oclIsKindOf(CV_Grid))
  * domainIsRectifiedGrid: The domain shall be a rectified grid. (OCL: inv: domainSet.oclIsKindOf(CV_RectifiedGrid)
  * grid points shall coincide with grid cell centres: Grid points of a RectifiedGridCoverage shall coincide with the centres of cells of the geographical grids defined in Section 2.2 of Annex II at any resolution level.

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

