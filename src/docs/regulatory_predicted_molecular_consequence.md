# Regulatory Predicted Molecular Consequence

| Field             | Type            | Description
|-------------------|-----------------|---------------------
|allele_name|string|Data-derived allele name
|stable_id|string|Feature stable id
|feature_type|OntologyTermMetadata|SO term for feature type (eg. transcript, regulatory features like promoter)
|consequences|array of OntologyTermMetadata|SO terms for predicted impact ( eg regulatory_region_variant)
|regulatory_feature_relative_location|VariantRelativeLocation|Relative location on regulatory feature


```json
"name": "rs1761454157",
"alleles":  [
    {
    "name": "5:173235220:G:A",
    "predicted_molecular_consequences": [],
    "regulatory_predicted_molecular_consequences": [{
        "allele_name": "A",
        "stable_id": "ENSR5_94JQHZ",
        "feature_type": {
            "value": "promoter"
            },
        "consequences": [
            {
            "value": "regulatory_region_variant"
            }
        ],             
        "regulatory_feature_relative_location": {
            "start": 25,
            "end": 25,
            "length": 1,
            "ref_sequence": "G",   
            "alt_sequence": "A"
        },
    }],
    "motif_predicted_molecular_consequences": []
    }
]
```