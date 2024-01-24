# Population

A group of samples which have been studied and are logical to consider together

| Field             | Type            | Description
|-------------------|-----------------|---------------------
| name              | string          | Name of the population
| size              | integer         | Size of the population (maximum size)
| description       | string          | Description of the population
| type              | ValueSet        | Type of population e.g. based on geography or collection of individuals/samples
| is_global            | boolean         | Is this a population that can be used to report global minor allele frequency
| is_from_genotypes| boolean         | frequency from genotypes or from individuals/sample genotypes
| display_group_name| string          | The name of the group of populations this population belongs to, serves as a table header on population genetics page
| super_population  | Population or null     | Super population if exists
| sub_populations    | array of Population or [ ]    | Sub population if exists























