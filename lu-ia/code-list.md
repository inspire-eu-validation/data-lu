# Code lists

**Purpose**: Verify that code lists extensions can be accessed.

**Prerequisites**

**Test method**

* Verify that any code list extensions are publicly accessible via HTTP, i.e. inspect extensible code list valued property elements. If a reference (@xlink:href) has a value that does not start with http://inspire.ec.europa.eu/codelist/, verify that a HTTP GET request to the URI retrieves a document. Otherwise report [brokenLink](#brokenLink).

This data theme currently has the following extensible code lists:

* [LandUseClassificationValue](#LandUseClassificationValue) : http://inspire.ec.europa.eu/codelist/LandUseClassificationValue

* [PlanTypeNameValue](#PlanTypeNameValue) : http://inspire.ec.europa.eu/codelist/PlanTypeNameValue

* [SpecificSupplementaryRegulationValue](#SpecificSupplementaryRegulationValue) :  http://inspire.ec.europa.eu/codelist/SpecificSupplementaryRegulationValue

* [SupplementaryRegulationValue](#SupplementaryRegulationValue) : http://inspire.ec.europa.eu/codelist/SupplementaryRegulationValue

**Reference(s)**: 

* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 6 (3)

**Test type**: Automated

**Notes**

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
brokenLink <a name="brokenLink"/>  |  XML document '$filename', $featureType '$gmlid': The property '$propertyName' has a value '$value' that cannot be retrieved using HTTP. Every code list value must be made available in an online registry. 

## Contextual XPath references

The namespace prefixes used as described in [README](./README.md#namespaces).

Abbreviation                                               |  XPath expression      |Multiplicity   |Voidable
---------------------------------------------------------- | -----------------------|---------------|---------------------------------
LandUseClassificationValue <a name ="LandUseClassificationValue"></a>	| //schema-element(\*:\*)/lunom:orderedList/@xlink:href <br> //schema-element(\*:\*)/lunom:specificValue/@xlink:href <br> //schema-element(\*:\*)/\:specificLandUse/@xlink:href | 1..\* <br> 1 <br> 1..\* | No <br> No <br> Yes
PlanTypeNameValue <a name ="PlanTypeNameValue"></a>	| //schema-element(\*:\*)/\*:planTypeName/@xlink:href | 1 | No  
SpecificSupplementaryRegulationValue <a name ="SpecificSupplementaryRegulationValue"></a>	| //schema-element(\*:\*)/\*:specificSupplementaryRegulation/@xlink:href | 1..\* | Yes
SupplementaryRegulationValue <a name ="SupplementaryRegulationValue"></a>	| //schema-element(\*:\*)/\*:supplementaryRegulation/@xlink:href | 1..\* | No
