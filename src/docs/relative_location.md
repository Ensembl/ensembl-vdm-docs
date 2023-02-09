# Relative Location

It is important to know where in a genomic feature a variant lies and in the case of longer variants what proportion of the feature is overlapped (express as fraction of genomic feature not variant)

| Field             | Type            | Description
|-------------------|-----------------|---------------------
| Subject           | Feature         | The feature we are interested in, for example a VariantAllele
| Object            | Feature / Sequence| A reference feature sequence the subject overlaps eg. a transcript
| relation          | enum (overlaps, upstream, downstream) | Type of relative location 
| start             | int             |Start of subject within object. May be negative if upstream 
| end               | int             | End of subject within object 
| length            | int             | Length of overlap
| percentage_overlap| float           | Percentage of object overlapped by the subject (Of particular interest for structural variants)

## Questions/Comments
* Is the name of the data type too generic?
* Can `Subject` be limited to allele?
* Why is `Object` a `Sequence`? Is protein not a `Feature`? 
* For `Object`, how do we refer to the CDS of the transcript: Ex: ENST00000679684.1_cds











