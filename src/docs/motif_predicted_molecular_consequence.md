# Motif Predicted Molecular Consequence

| Field             | Type            | Description
|-------------------|-----------------|---------------------
|allele_name|string|Data-derived allele name
stable_id|string|Feature stable id
|feature_type|OntologyTermMetadata|SO term for feature type (eg. transcript, regulatory feature, motif feature)
|consequences|array of OntologyTermMetadata|SO terms for predicted impact ( eg TF_binding_site_variant)
|binding_matrix_stable_id|string|Binding matrix stable id
|motif_feature_relative_location|VariantRelativeLocation or null|Relative location on motif feature
|motif_score_delta|float|The deviation from the score (that is derived from alignment software (e.g. MOODS)) caused by the variation.
|in_informative_position|boolean|Flags if the variation is in an informative position.

```json
"name": "rs144601450",
"alleles":  [{
    "name": "Y:56673840:G:C",
    "predicted_molecular_consequences": {},
    "regulatory_predicted_molecular_consequences": {},
    "motif_predicted_molecular_consequences": {
        "allele_name": "C",
        "stable_id": "ENSM00001002745",
        "feature_type": {
            "value": "Motif Feature"
            },
        "consequences": [
            {
            "value": "TF_binding_site_variant"
            }
        ],
        "binding_matrix_stable_id": "ENSPFM0352",
        "motif_feature_relative_location": {
            "start": 5,
            "end": 5,
            "length": 1,
            "ref_sequence": "G",   
            "alt_sequence": "C"
        },
        "motif_score_delta": -0.080969,
        "in_informative_position": true
                          
    }
}]
```