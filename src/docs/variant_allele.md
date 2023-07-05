# Variant Allele
An allele is a precise entity. It represents an assertion of the state of a biological sequence at a location. It is a Feature. 
It does not have a stable_id and version fields - like an intron

| Field             | Type            | Description
|-------------------|-----------------|---------------------
| name               | string         | Name of the allele - using position based format - SPDI (not necessarily normalised)
| allele_sequence    |  string               | Alternative allele with respect to this sequence/ slice
| reference_sequence |  string        | Reference allele with respect to this sequence/ slice
| alternative_names  | array of External Reference or [ ] | Alternative names + source info
| type               | string                     | This is always VariantAllele
| allele_type        | OntologyTermMetadata| SO type eg. insertion, deletion
| slice              | Slice                      | Slice describing the coordinates of the allele
| population_frequencies| array of PopulationAlleleFrequency or []| Shows rate of occurrence in different populations. Can be empty
| phenotype_assertions| array of Phenotype Assertion or []| Links to disease where the precise allele is known. Can be empty
| prediction_results | array of PredictionResults or []| These are results at variant allele/loci level CADD
| predicted _molecular_consequences| Array of PredictedMolecularConsequence or []| Shows predicted  effect on transcripts, regulatory features etc. Can be empty























