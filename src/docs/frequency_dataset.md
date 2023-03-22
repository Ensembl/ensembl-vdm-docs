# Frequency Dataset

* Dataset used to extract frequency data from.
* Usually a VCF file; in future may be a EVA study
* Should cache file be considered derived frequency set
* This must have appropriate ids to link to the info in the DataFiles API; only info used for display is help here, not info on how to obtain the data
* Is this a subset of DataSet - TDB - review work done by Production

| Field             | Type            | Description
|-------------------|-----------------|---------------------
| version           | string          | 
| release_date      | string          | YYYY-MM-DD
| source            | ExternalDB      | source of data set
| populations       | array of Population| Populations that make up this data set
| organism           | Organism         | 

## Changelog
* Removed datafile_id
* Changed species to organism
* Removed chromosomes
* Removed assembly




 



















