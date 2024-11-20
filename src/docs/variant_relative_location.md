# Variant Relative Location

It is important to know where in a genomic feature a variant lies and in the case of longer variants what proportion of the feature is overlapped (express as fraction of genomic feature not variant)

| Field             | Type            | Description
|-------------------|-----------------|---------------------
| relation          | ValueSet or null        | Type of relative location 
| start             | int or null             | Start of subject within object. May be null if intronic
| end               | int or null             | End of subject within object.  
| length            | int  or null          | Length of overlap. May be null if boundary is not known
| percentage_overlap| float or null         | Percentage of object overlapped by the subject (Of particular interest for structural variants)
| ref_sequence   | string or null          | Original sequence 
| alt_sequence   | string  or null        | New sequence 


Note: 
For `alt_sequence`, in case of frameshift variants, "X" would be easier to handle than any of the other options for now. In the future, we replace "X" with the new protein string.
In case of deletion, `alt_sequence` will be "-" 

In the case of variants with unknown start/end locations:
For example, "628-?",  
`start`: 628
`end`: null
`length`: null
`ref_sequence`: null
`alt_sequence`: null








