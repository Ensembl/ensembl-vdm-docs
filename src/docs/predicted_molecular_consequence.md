# Predicted Molecular Consequence

A set of information enabling interpretation of likely variant impact on genomic features such as transcripts and regulatory features

| Field             | Type            | Description
|-------------------|-----------------|---------------------
| allele_name           | string          | Data-derived allele name
| feature_stable_id | string          | Feature (eg transcript) id
| feature_type      | OntologyTermMetadata        | SO term for feature type (eg. transcript, regulatory feature)
| consequences      | array of OntologyTermMetadata           | SO terms for predicted impact ( eg missense variants)
| labels            | array of Label or [ ]  | Nomenclature values and source
| prediction_results | array of PredictionResult or [ ] | Scores from programs like SIFT which calculate transcript-specific deleteriousness scores
| relative_locations | array of VariantRelativeLocation or [ ] | 



























