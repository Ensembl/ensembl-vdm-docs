# Structural Variant 
Structural variant groups Structural Variant alleles. 


| Field             | Type            | Description
|-------------------|-----------------|---------------------
| name         | string          | Name of the variant from a known resource such as dbSNP, EVA, COSMIC
| alternative_names         |array of External Reference or [ ]        | Alternative names + source info
| primary_source     |ExternalReference      | Resource the initial record came from and where the name is assigned
| type               |string           |This is a StructuralVariant 
| allele_type        | OntologyTermMetadata| SO type aggregation from alleles 
| length             | int      | Aggregation from StructuralVariantAllele
| slice              | Slice                      | Slice describing the max coordinates of all the alleles for the variant
| prediction_results | array of PredictionResults or [ ] | These are results at variant/loci level GERP, AA
| alleles |array of StructuralVariantAllele |List of VariantAlleles
| citations| array of Publications or [ ] |List of Publications
| phenotype_assertions| array of PhenotypeAssertion or [ ] |Links to disease where the precise allele is unknown
| ensembl_website_display_data| VariantDisplayData | Display data required for Ensembl Website at a Variant level