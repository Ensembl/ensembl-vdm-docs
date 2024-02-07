# Variant Relative Location

It is important to know where in a genomic feature a variant lies and in the case of longer variants what proportion of the feature is overlapped (express as fraction of genomic feature not variant)

| Field             | Type            | Description
|-------------------|-----------------|---------------------
| relation          | ValueSet        | Type of relative location 
| start             | int             | Start of subject within object. May be negative if upstream 
| end               | int             | End of subject within object 
| length            | int             | Length of overlap
| percentage_overlap| float           | Percentage of object overlapped by the subject (Of particular interest for structural variants)
| sequence_change   | string          | Sequence change based on the overlapping feature












