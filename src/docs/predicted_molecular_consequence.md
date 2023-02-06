# Predicted Molecular Consequence

A set of information enabling interpretation of likely variant impact on genomic features such as transcripts and regulatory features

| Field             | Type            | Description
|-------------------|-----------------|---------------------
| allele            | string          | Data-derived allele name
| feature_stable_id | string          | Feature (eg transcript) id
| feature_type      | string          | SO term for feature type (eg. transcript, regulatory feature)
| consequences      | list            | SO terms for predicted impact ( eg missense variants)
| labels            | array of Label  | Nomenclature values and source
| prediction_results | array of PredictionResult | Scores from programs like SIFT which calculate transcript-specific deleteriousness scores
| overlaps           | list of OverlapStatement | Description of overlap of allele with feature
| relative_location(s) | Array of RelativeLocation | 

















