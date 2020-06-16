# Feature references

**Purpose**: Verify that referenced features can be retrieved.

**Prerequisites**

**Test method**

* Verify that any feature reference in an association role is publicly accessible via HTTP, i.e. inspect all relevant properties. If a reference (@xlink:href) has a value that starts with "#", verify that an element with a `gml:id` attribute with the referenced identifier exists in the same document. If the reference starts with "http", verify that a HTTP GET request to the URI retrieves an XML document. Otherwise report [brokenLink](#brokenLink).

This data theme currently has the following association roles:

* ExistingLandUseDataSet.[member](#elumember): ExistingLandUseObject
* ExistingLandUseObject.[dataset](#dataset): ExistingLandUseDataSet
* SpatialPlan.[member](#plumember): ZoningElement
* SpatialPlan.[officialDocument](#pluofficialDocument1): OfficialDocumentation
* SpatialPlan.[restriction](#restriction): SupplementaryRegulation
* ZoningElement.[plan](#plan): SpatialPlan
* ZoningElement.[officialDocument](#pluofficialDocument2): OfficialDocumentation
* SupplementaryRegulation.[plan](#plan2): SpatialPlan
* SupplementaryRegulation.[officialDocument](#pluofficialDocument3): OfficialDocumentation
* SampledExistingLandUseDataSet.[member](#selumember): ExistingLandUseSample
* ExistingLandUseSample.[dataset](#seludataset): SampledExistingLandUseDataSet

**Reference(s)**: 

* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 4 (2)

**Test type**: Automated

**Notes**

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
brokenLink <a name="brokenLink"/>  |  XML document '$filename', $featureType '$gmlid': The property '$propertyName' has a value '$value' that cannot be retrieved using HTTP. Every code list value must be made available in an online registry. 

## Contextual XPath references

The namespace prefixes used as described in [README](./README.md#namespaces).

Abbreviation                                               |  XPath expression    | Multiplicity    | Voidable
---------------------------------------------------------- | ---------------------|-----------------|------------
member <a name ="elumember"></a>	| //schema-element(elu:ExistingLandUseDataSet)/elu:member/@xlink:href | 0..\* | No
dataset <a name ="dataset"></a>	| //schema-element(elu:ExistingLandUseObject)/elu:dataset/@xlink:href | 1 | No
member <a name ="plumember"></a>	| //schema-element(plu:SpatialPlan)/plu:member/@xlink:href | 0..\* | No
officialDocument <a name ="pluofficialDocument1"></a>	| //schema-element(plu:SpatialPlan)/plu:officialDocument/@xlink:href | 1..\* | Yes
restriction <a name ="restriction"></a>	| //schema-element(plu:SpatialPlan)/plu:restriction/@xlink:href | 0..\* | No
plan <a name ="plan"></a>	| //schema-element(plu:SupplementaryRegulation)/plu:plan/@xlink:href | 1 | No
officialDocument <a name ="pluofficialDocument2"></a>	| //schema-element(plu:ZoningElement)/plu:officialDocument/@xlink:href | 1..\* | Yes
plan <a name ="plan2"></a>	| //schema-element(plu:SupplementaryRegulation)/plu:plan/@xlink:href | 1 | No
officialDocument <a name ="pluofficialDocument3"></a>	| //schema-element(plu:SupplementaryRegulation)/plu:officialDocument/@xlink:href | 1..\* | Yes
member <a name ="selumember"></a>	| //schema-element(selu:SampledExistingLandUseDataSet)/selu:member/@xlink:href | 0..\* | No
dataset <a name ="seludataset"></a>	| //schema-element(elu:ExistingLandUseSample)/selu:dataset/@xlink:href | 1 | No
