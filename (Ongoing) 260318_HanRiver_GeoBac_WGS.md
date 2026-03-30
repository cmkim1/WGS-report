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
* Taxonomic identification was conducted based on 16S rRNA sequences.


Statistics | C2 | C3 | C4 | C5 | P1 | P2 | A3
---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- 
Number of contigs | 90 | 52 | 50 | 81 | 1 | 2 | 1
Total assembly length (bp) | - | - | - | - | 5,275,989 | 6,292,670 | 8,718,636
Genome coverage | - | - | - | - | 155x | 133x | 27x
Circular | - | - | - | - | Y | Y | N
Genome completeness (%) | 98.28 | 100 | 100 | 100 | 100 | 99.67 | 99.49
Genome contamination (%) | **93.75** | **191.67** | **203.12** | **183.65** | 0.33 | 0.96 | 1.64
16s based identification | - | - | - | - | **_Massilia aurea_** | **_Janthinobacterium aestuarii_** | **_Streptomyces venezuelae_**

## Mixed genome binning

* Binning was performed using MetaBAT2.
* Each sample was binned into four bins.

| Statistics | C2 | C3 | C4 | C5 |
| ---- | ---- | ---- | ---- | ---- |
| bin1completeness (%) | 99.54 | - | 99.00 | 57.58 |
| bin1contamination (%) | 1.10 | - | 0.45 | 0.31 |
| bin1 16S identification | _Arenimonas aquatica_ | - | _Rhodobacter amnigenus_ | _Allobosea minatitlanensis_ |
| bin2completeness (%) | - | 99.42 | - | - |
| bin2contamination (%) | - | 0.72 | - | - |
| bin2 16S identification | - | _Erythrobacter ramosus_ | - | - |
| bin3completeness (%) | 76.06 | 98.65 | 98.94 | 99.27 |
| bin3contamination (%) | 0 | 0 | 0 | 0 |
| bin3 16S identification | _Lacibacter koreensis_ | _Microcoleus anatoxicus_ / **_Phormidium nigroviride_** | _Microcoleus anatoxicus_ / **_Phormidium nigroviride_** | _Microcoleus anatoxicus_ / **_Phormidium nigroviride_** |
| bin4completeness (%) | 94.81 | 74.22 | 97.01 | 99.43 |
| bin4contamination (%) | 0.83 | 0.78 | 1.37 | 2.09 |
| bin4 16S identification | **_Pseudanabaena foetida_** | _Dyadobacter psychrophilus_ (94.57) | _Neoroseomonas lacus_ | _Erythrobacter neustonensis_ |

## Odor compound synthesisizing genes



