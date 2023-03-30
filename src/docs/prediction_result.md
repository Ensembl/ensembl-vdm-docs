# Prediction Result

The result of a program like SIFT or GERP which can help interpret if a genomic change may be tolerated or pathogenic. This may be transcript or only genome dependent

| Field             | Type            | Description
|-------------------|-----------------|---------------------
| score             | float           | Numeric output of prediction package
| result            | string          | String output of prediction package
| classification    | ValueSet        | Text description of result eg tolerated
| analysis_method   | AnalysisMethod  | Tool, version and datasets used


## Changelog
* classification is ValueSet








