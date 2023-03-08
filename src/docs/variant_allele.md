# Variant Allele
An allele is a precise entity. It represents an assertion of the state of a biological sequence at a location. It is a Feature. 
It does not have a stable_id and version fields - like an intron

| Field             | Type            | Description
|-------------------|-----------------|---------------------
| name               | string          | Name of the allele - using position based format - SPDI (not necessarily normalised)
| allele_sequence    |                 | Alternative allele with respect to this sequence/ slice
| reference_sequence |                 | Reference allele with respect to this sequence/ slice
| alternative_names  | array of External Reference| Alternative names + source info
| type               | string                     | This is always VariantAllele
| allele_type        | OntologyTermMetadata| SO type eg. insertion, deletion
| slice              | Slice                      | Slice describing the coordinates of the allele
| population_frequencies| array of PopulationFrequency| Shows rate of occurrence in different populations. Can be empty
| phenotype_assertions| array of Phenotype Assertion| Links to disease where the precise allele is known. Can be empty
| predicted _molecular_consequences| Array of PredictedMolecularConsequence]| Shows predicted  effect on transcripts, regulatory features etc. Can be empty
| experimental_consequences| Array of ExperimentalConsequences| Placeholder for AVE (Atlas of Variant Effects) etc. Can be empty

## Questions/Comments :
* `Variant allele` is a `Feature`, should it have a stable_id? 
* `name` can be calulated as SPDI on the fly. Not Urgent?

## Changelog
* type is VariantAllele
* allele_type is OntologyTermMetadata




















