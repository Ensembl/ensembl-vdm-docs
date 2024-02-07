# Predicted Molecular Consequence

A set of information enabling interpretation of likely variant impact on genomic features such as transcripts and regulatory features

| Field             | Type            | Description
|-------------------|-----------------|---------------------
| allele_name           | string          | Data-derived allele name
| stable_id | string          | Feature stable id (transcripts for now)
| feature_type      | OntologyTermMetadata        | SO term for feature type (eg. transcript, regulatory feature)
| consequences      | array of OntologyTermMetadata           | SO terms for predicted impact ( eg missense variants)
| gene_stable_id | string| Gene stable id
| gene_symbol | string | Gene symbol
| protein_stable_id  | string or null | Protein stable id
| variant_representation | array of VariantRepresentation or [ ]  | Nomenclature values and source
| prediction_results | array of PredictionResult or [ ] | Scores from programs like SIFT which calculate transcript-specific deleteriousness scores
| transcript_biotype | string | Feature biotype
| cdna_location | VariantRelativeLocation  | Relative location on cDNA
| cds_location | VariantRelativeLocation or null | Relative location on CDS
| protein_location | VariantRelativeLocation or null | Relative location on protein

```
## Example for rs699 

"allele_name": "G",
"transcript_stable_id": "ENST00000680783",
"feature_type" : 
{
"accession_id": "SO:0000673",
"value": "transcript",
"url": "www.sequenceontology.org/browser/current_release/term/SO:0000673",
  "source": {
    "id": "...",
    "name": "Sequence Ontology",
    "url": "www.sequenceontology.org",
    "description": "The Sequence Ontology..."
  }
},

"consequences":
[{
  "accession_id": "SO:0001583",
  "value": "missense_variant",
  "url": "www.sequenceontology.org/browser/current_release/term/SO:0001583",
  "source": {
    "id": "...",
    "name": "Sequence Ontology",
    "url": "www.sequenceontology.org",
    "description": "The Sequence Ontology..."
  }
}],
"gene_stable_id" : "ENSG00000135744",
"gene_symbol": "AGT",
"protein_stable_id": "ENSP00000506329",
"variant_representation": 
{
	"representation": "ENST00000680783.1:c.776T>C",
	"naming convention": "HGVS",
	"qualifier": "coding"
},
"prediction_results": [] ,
"transcript_biotype": "protein_coding",
"cdna_location": 
{
	"relation": "overlaps" ,
	"start": 1287,
	"end": 1287, 
	"length": 1, 
	"percentage_overlap": 1.0,
	"sequence_change": "T/C" 
},
"cds_location": 
{
	"relation": "overlaps" ,
	"start": 776, 
	"end": 776, 
	"length": 1, 
	"percentage_overlap": 1.0,
	"sequence_change": "ATG/ACG" 
},
"protein_location":
{
	"relation": "overlaps" ,
	"start": 259, 
	"end": 259, 
	"length": 1, 
	"percentage_overlap": 1.0 ,
	"sequence_change": "M/T" 
}
```



























