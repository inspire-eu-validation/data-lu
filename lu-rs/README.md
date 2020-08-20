# Conformance class: Reference systems, Land Use

Conformance class for the requirements associated with reference systems (spatial and temporal, units of measurement).

To be able to test this conformance class, the encoding of the data set must be known, i.e. this is a parameterized conformance class. The XPath expressions used in this test suite assume that the GML encoding is used. If used with the GML encoding this conformance class has an indirect dependency to the conformance class "GML application schema for Land Use".

This conformance class is part of the [INSPIRE Data Specification on Land Use](../README.md).

## Standardization target type

INSPIRE spatial data set

## Dependencies

### Direct dependencies

A direct dependency is another conformance class whose requirements must be met by the data set, too.

| Specification | Conformance class | Parameters | 
| ------------- | ----------------- | ---------- |
| [TG DS Template](#ref_TG_DS_tmpl) | [Reference systems](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/reference-systems) | n/a |

### Indirect dependencies

An indirect dependency is another conformance class whose requirements must be met by a related resource.

| Specification | Conformance class | Related resource | Parameters |
| ------------- | ----------------- | ---------------- | ---------- |
| [TG DS-LU](#ref_TG_DS_LU) | [GML application schema, Land Use](../lu-gml/README.md) | INSPIRE spatial data set encoded in GML, Land Use features | n/a |
 
## Feature types <a name="feature-types"></a>

The instantiable feature types are:
 
Existing Land Use:
* ExistingLandUseDataSet
* ExistingLandUseObject

Gridded Existing Land Use:
* ExistingLandUseGrid

Planned Land Use:
* SpatialPlan
* SupplementaryRegulation
* ZoningElement
* OfficialDocumentation

Sampled Existing Land Use:
* SampledExistingLandUseDataSet
* ExistingLandUseSample
 
*Note*: When "features" or "spatial objects" are mentioned in the test cases, this refers only to instances of feature types of this application schema, not to any types specified in any other application schema.

## External document references

The following abbreviations are used in the test text for referring to external documents:

Abbreviation                     | Document name
-------------------------------- | --------------------------------------------------
TG DS-LU <a name="ref_TG_DS_LU"></a>   | [INSPIRE Data Specification on Land Use – Technical Guidelines version 3.2](http://inspire.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_LU_v3.0.pdf)
TG DS Template <a name="ref_TG_DS_tmpl"></a>   | [INSPIRE Data Specification Template version 3.0rc3](http://inspire.jrc.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_Template_v3.0rc3.pdf)

## Tests

This Conformance Class contains the following tests.

| Identifier                                                                          | Status   |
| ----------------------------------------------------------------------------------- | -------- |
| [Projection](./projection.md) | Ready for review |

## XML namespace prefixes <a name="namespaces"></a>

n/a
