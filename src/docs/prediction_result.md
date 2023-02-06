# Prediction Result

The result of a program like SIFT or GERP which can help interpret if a genomic change may be tolerated or pathogenic. This may be transcript or only genome dependent

| Field             | Type            | Description
|-------------------|-----------------|---------------------
|score              | float           | Numeric output of prediction package
| classification    | string or null  | Text description of result eg tolerated
| tool              | string          | Program name eg PolyPhen-2
| qualifier         | string or null  | Mode of use/ type of result eg HumVar or HumDiv for Polyhen-2, raw or PRED style for CADD
| version           | string          | Version of program
| datasets          | Array of DataSet| Datasets used in the analysis eg UniRef90 for SIFT











