# Phenotype assertion

An assertion that a genomic feature has been assayed for involvement in a disease, trait or phenotype

| Field             | Type            | Description
|-------------------|-----------------|---------------------
| feature           | Feature          | Feature name
| feature_type      | string          | SO term for feature type (eg.Gene, VariantAllele, variant)
| phenotype         | Phenotype       | Where possible this is a term from ontology such as HPO eg. ‘Renal dysplasia’ but this is not always possible
| evidence          | Array of Evidence| Evidence sets supporting this assertion

## Questions/Comments
* Can we have a better name for `phenotype` ? We dump traits and diseases together. Not Urgent


