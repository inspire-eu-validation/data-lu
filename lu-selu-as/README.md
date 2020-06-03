# Conformance class: Application schema, Sampled Existing Land Use

Conformance class for the requirements associated with the application schema. 

To be able to test this conformance class, the encoding of the data set must be known, i.e. this is a parameterized conformance class. The XPath expressions used in this test suite assume that the GML encoding is used. If used with the GML encoding this conformance class has an indirect dependency to the conformance class "GML application schemas, Land Use".

This conformance class is part of the [INSPIRE Data Specification on Land Use](../README.md).

## Standardization target type

INSPIRE spatial data set

## Dependencies

### Direct dependencies

none

### Indirect dependencies

An indirect dependency is another conformance class whose requirements must be met by a related resource.

| Specification | Conformance class | Related resource | Parameters |
| ------------- | ----------------- | ---------------- | ---------- |
| [TG DS-lu](./README.md#ref_TG_DS_LU) | [GML application schemas, Land Use](../lu-gml/README.md) | INSPIRE spatial data set encoded in GML, Land Use features | n/a |
 
## Feature types <a name="feature-types"></a>

The instantiable feature types in the application schema are:

* TO BE COMPLETED


*Note*: When "features" or "spatial objects" are mentioned in the test cases, this refers only to instances of feature types of this application schema, not to any types specified in any other application schema.

## External document references

The following abbreviations are used in the test text for referring to external documents:

Abbreviation                     | Document name
-------------------------------- | --------------------------------------------------
TG DS-lu <a name="ref_TG_DS_LU"></a>   | [INSPIRE Data Specification on Land Use – Technical Guidelines version 3.0](http://inspire.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_LU_v3.0.pdf)
TG DS Template <a name="ref_TG_DS_tmpl"></a>   | [INSPIRE Data Specification Template version 3.0rc3](http://inspire.jrc.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_Template_v3.0rc3.pdf)

## Test Cases

| Identifier                                                        | Status   | Test case in [TG DS-lu](#ref_TG_DS_LU)  |
| ----------------------------------------------------------------- | -------- | ------------ |
| [Code list values](./code-list-values.md)  | Draft  | A.1.3  |

## XML namespace prefixes <a name="namespaces"></a>

The following prefixes are used to refer to the corresponding XML namespaces in all test descriptions:

Prefix         | Namespace
-------------- | -------------------------------------------------
lu             | http://inspire.ec.europa.eu/schemas/lu/4.0
net            | http://inspire.ec.europa.eu/schemas/net/4.0
base           | http://inspire.ec.europa.eu/schemas/base/3.3
gml            | http://www.opengis.net/gml/3.2
wfs            | http://www.opengis.net/wfs/2.0
xsi            | http://www.w3.org/2001/XMLSchema-instance
xlink          | http://www.w3.org/1999/xlink
xml            | http://www.w3.org/XML/1998/namespace
