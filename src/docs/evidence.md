# Evidence ( of Disease/Phenotype assertion)

| Field             | Type            | Description
|-------------------|-----------------|---------------------
| source            | ExternalDB         | The original database reporting the assertion eg ClinVar, OMIA
| assertion         | ValueSet (pathogenic, benign etc)| High level assertion result eg Pathogenic from ClinVar
| attributes        | array of Attribute | Different databases and experimental methods report different information about an assertion
| citations         | array of strings | May be PMID, PMCid or DOI

## Questions/Comments
* Should `source` be ExternalDB similar to `variant.primary_source`?
* Can we model citations better instead of strings (PMID:12345) ?





