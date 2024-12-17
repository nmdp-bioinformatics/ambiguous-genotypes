# ambiguous-genotypes
sample data with ambiguous genotypes and the corresponding unambiguous genotype


-----

`ambig.csv.gz` a csv file with four columns:

-   id
-   glstring-unambig
-   glstring-ambig
-   race

It can be used to test software that disambiguates HLA.
There are two forms of ambiguity: missing loci and allele ambiguity.

The file contains a header and 40,000 data rows.

Here is a summary by race:

| count | race      |
| ------|-----      |
| 14000 | AAFA      |
|  3000 | CARB      |
|  7000 | FILII     |
|  7000 | MENAFC    |
|  9000 | EURCAU    |


1. "id" is an identifier.

example: `ID00000001`

2. "glstring-unambig" is an unphased, unambiguous glstring [1]

example: `A*01:02+A*30:01^B*42:02+B*49:01^C*07:01+C*17:01^DQB1*05:01+DQB1*05:01^DRB1*01:02+DRB1*13:02`

3. "glstring-ambig" is an unphased, ambiguous glstring [1]

example: `A*23:01/A*23:02/A*23:03/A*23:04/A*23:05/A*23:06/A*23:08N/A*23:09/A*23:10/A*23:11N/A*23:12/A*23:13/A*23:14/A*23:15/A*23:16/A*23:19Q/A*23:21/A*23:22/A*23:23/A*23:24/A*23:25/A*23:26/A*23:27/A*23:28/A*23:29/A*23:30/A*23:31/A*23:32/A*23:33/A*23:34/A*23:35/A*23:36/A*23:37/A*23:38N/A*23:39/A*23:40/A*23:41/A*23:42/A*23:43/A*23:44/A*23:45/A*23:46/A*23:47/A*23:48/A*23:49/A*23:50/A*23:51/A*23:52/A*23:53/A*23:54/A*23:55/A*23:56/A*23:57/A*23:59/A*23:60+A*80:01/A*80:02/A*80:03^B*45:01/B*45:02/B*45:03/B*45:04/B*45:05/B*45:06/B*45:08/B*45:09/B*45:10/B*45:11/B*45:12/B*45:14+B*78:01/B*78:02/B*78:03/B*78:04/B*78:05/B*78:06/B*78:07`

4. "race" is a string that identifies the race/ethnicity of the indiviual [2]

example: EURCAU 

### References

[1] PMID: 37403548

[2] PMID: 23806270
