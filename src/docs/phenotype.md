# Phenotype

| Field             | Type            | Description
|-------------------|-----------------|---------------------
| name              | string          | Name of the phenotype/ disease/ trait 
| source            | ExternalDB      | Resource the initial record came from and where the name is assigned
| ontology_terms    | array of ExternalReference or [ ] | Terms from HPO, MONDO, or EFO which describe this phenotype/ disease/ trait. May be empty if no mapping 
