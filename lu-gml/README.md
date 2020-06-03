# Conformance class: GML application schemas, Land Use (DRAFT)

Conformance class for the GML encoding of spatial objects specified in the INSPIRE GML application schema 'Land Use'. This conformance class examines the data set against requirements associated with the GML application schema.

This conformance class is part of the [INSPIRE Data Specification on Land Use](../README.md).

## Standardization target type

INSPIRE spatial data set encoded in GML, Land Use features

## Dependencies

### Direct dependencies

A direct dependency is another conformance class whose requirements must be met by the GML documents, too.

| Specification | Conformance class | Parameters | 
| ------------- | ----------------- | ---------- |
| [TG DS Template](#ref_TG_DS_tmpl) | [INSPIRE GML application schemas](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/schemas) | n/a |

### Indirect dependencies

n/a
 
## External document references

The following abbreviations are used in the test text for referring to external documents:

Abbreviation                     | Document name
-------------------------------- | --------------------------------------------------
TG DS-lu <a name="ref_TG_DS_LU"></a>   | [INSPIRE Data Specification on Land Use – Technical Guidelines version 3.1](https://inspire.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_LU_v3.0.pdf)
TG DS Template <a name="ref_TG_DS_tmpl"></a>   | [INSPIRE Data Specification Template version 3.0rc3](http://inspire.jrc.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_Template_v3.0rc3.pdf)

## Test Cases

| Identifier                                                        | Status   | Test case in [TG DS-lu](#ref_TG_DS_LU)  |
| ----------------------------------------------------------------- | -------- | ------------ |
| [Basic test](./basic.md)  | ready for review  | A.1.1, (A.6.1)  |

## XML namespace prefixes <a name="namespaces"></a>

The following prefixes are used to refer to the corresponding XML namespaces in all test descriptions:

Prefix         | Namespace
-------------- | -------------------------------------------------
am          | http://inspire.ec.europa.eu/schemas/lu/4.0
