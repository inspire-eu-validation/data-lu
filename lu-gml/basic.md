# Basic test

**Purpose**: Verify that the spatial data set contains at least one Land Use feature.

**Prerequisites**

**Test method**

* Check that the set of [features](#features) in the spatial data set is not empty. Otherwise report [noFeature](#noFeature)

**Reference(s)**: 

* [TG DS-lu](./README.md#ref_TG_DS_LU) 5.4, 5.5

**Test type**: Automated

**Notes**

There is no requirement that we could reference in the Technical Guidelines. Maybe such a requirement should be added in the future revision?

## Messages

Identifier  |  Message text (parAMeters start with '$')
----------- | -------------------------------------------------------------------------
noFeature <a nAMe="noFeature"/>  |  	The XML documents representing the spatial data set do not contain a feature of any of the spatial object types in the 'Land Use - Land Use' or 'Land Use - Maritime Units' application schemas. Therefore, the spatial data set cannot conform to this conformance class. If you have expected to find spatial objects from the application schema in the data set, please consult the statistics information to see the spatial object types that have been found.

## Contextual XPath references

The namespace prefixes used as described in [README.md](./README.md#nAMespaces).

Abbreviation                                          |  XPath expression
----------------------------------------------------- | ------------------------------------------------------------------
features <a name="features"></a>   |  //schema-element(am:ManagementRestrictionOrRegulationZone) \|
