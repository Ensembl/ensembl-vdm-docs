# Population Allele Frequency

The frequency of an allele in a population

| Field             | Type            | Description
|-------------------|-----------------|---------------------
| population_name        | string          | Name of the population (used by PopulationAPI)
| allele_count      | integer or null | Number of individuals/samples in the population where variant allele is found
| allele_number     | integer or null | Total number of alleles in called genotypes
| allele_frequency  | float   | Frequency of this allele in the population
| dataset           | FrequencyDataset or null| Dataset from which frequency extracted
| qc_filter            | ValueSet or null | Used for filtering the frequencies e.g. only select those that have value PASS
| is_minor_allele      | boolean   | Is this allele a minor allele for the population and associated data set
| is_hpmaf             | boolean  | Is this allele a minor allele for the highest population and associated data set















