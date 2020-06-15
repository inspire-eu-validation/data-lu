# Code list values

**Purpose**: Verify whether all attributes whose value type is a code list take the values set out therein

**Prerequisites**

**Test method**

The following check is performed for every feature in the dataset.

* [Range](rangeSet) is based on either HILUCS or on a specific land use classification system defined by the data provider.

| https://inspire.ec.europa.eu/codelist/HILUCSValue | 

**Reference(s)**: 

* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 4 (1)
* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 4 (3)
* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 6 (1)
* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 6 (2)
* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 6 (3)
* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 6 (4)

**Test type**: Manual

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
disallowedCodeListValue <a name="disallowedCodeListValue"/>  |  XML document '$filename', $featureType '$gmlid': The property '$propertyName' has a value '$value' that is not one of the allowed values listed at $codelist. 

## Contextual XPath references

The namespace prefixes used as described in [README](./README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
rangeSet <a name="rangeSet"></a> 	| 	//schema-element(gelu:ExistingLandUseGrid)/gml:rangeSet/gml:CategoryList
