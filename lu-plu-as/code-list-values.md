# Code list values

**Purpose**: Verify whether all attributes whose value type is a code list take the values set out therein

**Prerequisites**

**Test method**

The following check is performed for every feature in the dataset.

* Check that all the [hilucsLandUse](#hilucsLandUse) elements has a xlink:href attribute pointing to a [valid value](#validValue). If the check fails report [disallowedCodeListValue](#disallowedCodeListValue).

| <a name="validValue"></a> Valid values for xlink:href attribute of [hilucsLandUse](#hilucsLandUse) element are available in the INSPIRE Registry| 
| ---- | 
| https://inspire.ec.europa.eu/codelist/HILUCSValue | 

* Check that all the [levelOfSpatialPlan](#levelOfSpatialPlan) elements has a xlink:href attribute pointing to a [valid value](#validValue). If the check fails report [disallowedCodeListValue](#disallowedCodeListValue).

| <a name="validValue"></a> Valid values for xlink:href attribute of [levelOfSpatialPlan](#levelOfSpatialPlan) element are available in the INSPIRE Registry| 
| ---- | 
| http://inspire.ec.europa.eu/codelist/LevelOfSpatialPlanValue | 

* Check that all the [processStepGeneral](#processStepGeneral) elements has a xlink:href attribute pointing to a [valid value](#validValue). If the check fails report [disallowedCodeListValue](#disallowedCodeListValue).

| <a name="validValue"></a> Valid values for xlink:href attribute of [processStepGeneral](#processStepGeneral) element are available in the INSPIRE Registry| 
| ---- | 
| http://inspire.ec.europa.eu/codelist/ProcessStepGeneralValue | 

* Check that all the [regulationNature](#regulationNature) elements has a xlink:href attribute pointing to a [valid value](#validValue). If the check fails report [disallowedCodeListValue](#disallowedCodeListValue).

| <a name="validValue"></a> Valid values for xlink:href attribute of [regulationNature](#regulationNature) element are available in the INSPIRE Registry| 
| ---- | 
| http://inspire.ec.europa.eu/codelist/RegulationNatureValue | 

**Reference(s)**: 

* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 4 (1)
* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 4 (3)
* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 6 (1)
* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 6 (2)
* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 6 (3)
* [TG DS Template](./README.md#ref_TG_DS_tmpl) IR requirement Article 6 (4)

**Test type**: Automated

**Notes**

The following is not applicable for this application schema as no extensions are allowed. It is still included here as a reminder in case extensions will be allowed in the future:

Inspect the code list valued property elements. If a value is not one of the values listed above, review the code list definition to check that any extensions do not overlap with the code lists that are defined in Annexes II, III and IV of the Implementing Rule and that all extensions conform to the requirements. This is a manual test.

## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
disallowedCodeListValue <a name="disallowedCodeListValue"/>  |  XML document '$filename', $featureType '$gmlid': The property '$propertyName' has a value '$value' that is not one of the allowed values listed at $codelist. 

## Contextual XPath references

The namespace prefixes used as described in [README](./README.md#namespaces).

Abbreviation                                               |  XPath expression
---------------------------------------------------------- | -------------------------------------------------------------------------
hilucsLandUse <a name="hilucsLandUse"></a>   | //schema-element(plu:SpatialPlan)/plu:hilucsLandUse
levelOfSpatialPlan <a name="levelOfSpatialPlan"></a>   | //schema-element(plu:SpatialPlan)/plu:levelOfSpatialPlan
processStepGeneral <a name="processStepGeneral"></a>   | //schema-element(plu:SpatialPlan)/plu:processStepGeneral
regulationNature <a name="regulationNature"></a>   | //schema-element(plu:SpatialPlan)/plu:regulationNature
