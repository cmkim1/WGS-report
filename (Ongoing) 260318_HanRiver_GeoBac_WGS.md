# gDNA sequencing summary for 한강통합물환경센터

gDNA sequencing was performed with Oxford Nanopore MinION platform.

* Library preparation, sequencing: Chungmin Kim
* Genome assembly, QC: Chungmin Kim

## Sequencing summary

Statistics | C2 | C3 | C4 | C5 | P1 | P2 | A3
---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- 
Total number of reads (k) | 78 | 306 | 362 | 275 | 304 | 244 | 108
Total number of bases (Mbp) | 232 | 657 | 719 | 490 | 1,066 | 1,045 | 320
Read N50 | 7,638 | 5,378 | 4,468 | 5,684 | 7,182 | 9,206 | 6,297
Median read quality score | 21.5 | 19.3 | 19.6 | 18.4 | 22.5 | 23 | 21.5


## Assembly summary

* Reads were filtered by minimum quality of 15 and minimum length of 3,000bp to generate genome with high completeness.
* Reads were assembled with [Flye genome assembler](https://github.com/fenderglass/Flye) v2.9.5 with `--nano-hq --iterations 2` parameters.
* Genome completeness were assessed with [checkM](https://github.com/Ecogenomics/CheckM) v1.2.4


Statistics | C2 | C3 | C4 | C5 | P1 | P2 | A3
---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- 
Number of contigs | 90 | 52 | 50 | 81 | 1 | 2 | 1
Total assembly length (bp) | - | - | - | - | 5,275,989 | 6,292,670 | 8,718,636
Genome coverage | - | - | - | - | 155x | 133x | 27x
Circular | - | - | - | - | Y | Y | N
Genome completeness (%) | 98.28 | 100 | 100 | 100 | 100 | 99.67 | 99.49
Genome contamination (%) | **93.75** | **191.67** | **203.12** | **183.65** | 0.33 | 0.96 | 1.64


