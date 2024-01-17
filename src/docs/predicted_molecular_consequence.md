# Predicted Molecular Consequence

A set of information enabling interpretation of likely variant impact on genomic features such as transcripts and regulatory features

| Field             | Type            | Description
|-------------------|-----------------|---------------------
| allele_name           | string          | Data-derived allele name
| feature_stable_id | string          | Feature (eg transcript) id
| feature_type      | OntologyTermMetadata        | SO term for feature type (eg. transcript, regulatory feature)
| consequences      | array of OntologyTermMetadata           | SO terms for predicted impact ( eg missense variants)
| gene_stable_id | string| Gene stable id
| gene_symbol | string | Gene symbol
| variant_representation | array of VariantRepresentation or [ ]  | Nomenclature values and source
| prediction_results | array of PredictionResult or [ ] | Scores from programs like SIFT which calculate transcript-specific deleteriousness scores
| transcript_biotype | string |
| cDNA_location | VariantRelativeLocation or null  | Relative location on cDNA
| CDS_location | VariantRelativeLocation or null | Relative location on CDS
| protein_location | VariantRelativeLocation or null | Relative location on protein



























