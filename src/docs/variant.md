# Variant

A variant is a conceptual entity which groups a set of alleles, similar to the way a gene groups one or more transcripts. (Do we need a canonical default position/allele)

A variant is not a feature as it does not have a precise single location but is slice and allele dependent. The same name is used across multiple assemblies and haplotypes.

| Field             | Type            | Description
|-------------------|-----------------|---------------------
|name         | string          | Name of the variant from a known resource such as dbSNP, EVA, COSMIC
|alternative_names         |array of External Reference         | Alternative names + source info
| primary_source     |ExternalDB       | Resource the initial record came from and where the name is assigned
| type|string |This is a Variant 
| prediction_results | array of PredictionResults | These are results at variant/loci level GERP, AA
|alleles |array of VariantAllele |List of VariantAlleles
| citations| array of Publications|List of Publications
| phenotype_assertions| array of PhenotypeAssertion|Links to disease where the precise allele is unknown


## Questions/Comments :
*  What is the best way to model citations? If citations are modeled as an array of ExternalReferences?

## Changelog
* citations is array of Publications
