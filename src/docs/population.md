# Population

A group of samples which have been studied and are logical to consider together

| Field             | Type            | Description
|-------------------|-----------------|---------------------
| population_id     | integer         | Unique internal identifier
| name              | string          | Name of the population
| size              | integer         | Size of the population (maximum size)
| description       | string          | Description of the population
| type              | ValueSet        | Type of population e.g. based on geography or collection of individuals/samples
| global            | boolean         | Is this a population that can be used to report global minor allele frequency
| frequency_from_gts| boolean         | frequency from genotypes or from individuals/sample genotypes
| display_group_name| string          | The name of the group of populations this population belongs to, serves as a table header
on population genetics page
| display_group_priority| integer     | Retrieves the priority of the group of populations this population belongs to, enabling the ordering of frequency data on the Population genetics page





















