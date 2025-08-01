# Structural Variant Allele
Currently models non-breakend SVs



| Field             | Type            | Description
|-------------------|-----------------|---------------------
| name               | string         | Name of the allele - from an accessioning repository(dbVar, DGVa)
| alternative_names  | array of External Reference or [] | Alternative names + source info
| type               | string                     | This is always StructuralVariantAllele
| allele_type        | OntologyTermMetadata| SO type eg. insertion, deletion
| slice              | Slice    | Slice describing the coordinates of the allele
| length             | int      | Length of the alternate variant allele
| copy_number        | integer or  null| For CNVs, the number of copies of the repeat unit present in this allele, otherwise null
| population_frequencies| array of PopulationAlleleFrequency or []| Shows rate of occurrence in different populations. Can be empty
| phenotype_assertions| array of PhenotypeAssertion or []| Links to disease where the precise allele is known. Can be empty
| prediction_results | array of PredictionResults or []| These are results at variant allele/loci level eg. CADD
| predicted_molecular_consequences| Array of PredictedMolecularConsequence or []| Shows predicted effect on transcripts



