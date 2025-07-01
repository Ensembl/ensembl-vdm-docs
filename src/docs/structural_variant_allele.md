# Structural Variant Allele
Currently models non-breakend SVs



| Field             | Type            | Description
|-------------------|-----------------|---------------------
| name               | string         | Name of the allele - from an accessioning repository(dbVar, DGVa)
| alternative_names  | array of External Reference or [] | Alternative names + source info
| type               | string                     | This is always StructuralVariantAllele
| allele_type        | OntologyTermMetadata| SO type eg. insertion, deletion
| slice              | Slice    | Slice describing the coordinates of the allele
| population_frequencies| array of PopulationAlleleFrequency or []| Shows rate of occurrence in different populations. Can be empty
| phenotype_assertions| array of Phenotype Assertion or []| Links to disease where the precise allele is known. Can be empty
| prediction_results | array of PredictionResults or []| These are results at variant allele/loci level CADD
| predicted_molecular_consequences| Array of PredictedMolecularConsequence or []| Shows predicted effect on transcripts
| experimental_consequences | array of ExperimentalConsequences or [] |Placeholder for AVE (Atlas of Variant Effects) etc.



