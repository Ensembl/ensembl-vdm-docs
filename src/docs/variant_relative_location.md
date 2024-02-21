# Variant Relative Location

It is important to know where in a genomic feature a variant lies and in the case of longer variants what proportion of the feature is overlapped (express as fraction of genomic feature not variant)

| Field             | Type            | Description
|-------------------|-----------------|---------------------
| relation          | ValueSet or null        | Type of relative location 
| start             | int             | Start of subject within object. May be negative if upstream 
| end               | int             | End of subject within object 
| length            | int             | Length of overlap
| percentage_overlap| float or null         | Percentage of object overlapped by the subject (Of particular interest for structural variants)
| ref_sequence   | string          | Original sequence 
| alt_sequence   | string          | New sequence 


Note: 
For `alt_sequence`, in case of frameshift variants, "X" would be easier to handle than any of the other options for now. In the future, we replace "X" with the new protein string.
In case of deletion, `alt_sequence` will be "-" 








