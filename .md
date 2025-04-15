# gDNA sequencing summary for Prof. D. Pathiraja

gDNA sequencing was performed with Oxford Nanopore MinION platform.

* Library preparation, sequencing: Chungmin Kim
* Genome assembly: Chungmin Kim

## Sequencing summary

Statistics | -
---- | ----
Total number of reads (k) | 302
Total number of bases (Mbp) | 291
Mean read length (bp) | 961.7
Mean read quality score | 17.9

## Assembly summary

* Reads with quality score over 20 were filtered to generate genome with high completeness.
* Reads were assembled with [Flye genome assembler](https://github.com/fenderglass/Flye) v2.9.5 with `--nano-hq --iterations 1` parameters.
* Completeness of assembled genome was assessed using [checkM](https://github.com/Ecogenomics/CheckM)


Statistics | -
---- | ----
Total assembly length (bp) | 4,437,548
Number of contigs | 10
Contig N50 (bp) | 1,176,033
Contig L50 | 2
GC ratio (%) | 45.5
Genome coverage | 28x
Genome completeness (%) | 99.81

## Species identification

* Average nucleotide identity was calculated using fastANI with reference genome seqeunces of Bacillus in NCBI.
* The genome was identified as _B. velezensis_, but it is also quite similar to _B. amyloliquefaciens_.

_G. Species_ | ANI
---- | ----
_B. velezensis_ | 98.0227
_B. amyloliquefaciens_ | 97.9505
_B. siamensis_ | 94.2418
