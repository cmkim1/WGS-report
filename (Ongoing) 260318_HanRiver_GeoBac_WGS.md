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
| bin1&nbsp;completeness&nbsp;(%) | 99.54 | - | 99.00 | 57.58 |
| bin1&nbsp;contamination&nbsp;(%) | 1.10 | - | 0.45 | 0.31 |
| bin1 16S identification | _Arenimonas aquatica_ | - | _Rhodobacter amnigenus_ | _Allobosea minatitlanensis_ |
| bin2&nbsp;completeness&nbsp;(%) | - | 99.42 | - | - |
| bin2&nbsp;contamination&nbsp;(%) | - | 0.72 | - | - |
| bin2 16S identification | - | _Erythrobacter ramosus_ | - | - |
| bin3&nbsp;completeness&nbsp;(%) | 76.06 | 98.65 | 98.94 | 99.27 |
| bin3&nbsp;contamination&nbsp;(%) | 0 | 0 | 0 | 0 |
| bin3 16S identification | _Lacibacter koreensis_ | _Microcoleus anatoxicus_ / **_Phormidium nigroviride_** | _Microcoleus anatoxicus_ / **_Phormidium nigroviride_** | _Microcoleus anatoxicus_ / **_Phormidium nigroviride_** |
| bin4&nbsp;completeness&nbsp;(%) | 94.81 | 74.22 | 97.01 | 99.43 |
| bin4&nbsp;contamination&nbsp;(%) | 0.83 | 0.78 | 1.37 | 2.09 |
| bin4 16S identification | **_Pseudanabaena foetida_** | _Dyadobacter psychrophilus_ (94.57) | _Neoroseomonas lacus_ | _Erythrobacter neustonensis_ |

## Odor compound synthesisizing genes
  
* Genomes were annotated using [prokka](https://github.com/tseemann/prokka) v1.14.6
* Odor compound synthesizing genes were searched using BLASTp.
* Carotenoid cleavage dioxygenase 1 from _Synechocystis_ sp., 2-methylisoborneol synthase from _Streptomyces venezuelae_ and geosmin synthase from _Coelosphaerium_ sp. G3 were used as queries.
* Odor compounds detected by GC in the samples are indicated in **bold**.

Compounds (gene) | C2&nbsp;Bin4 _Pseudanabaena&nbsp;foetida_ | C3&nbsp;Bin3 _Phormidium&nbsp;nigroviride_ | C4&nbsp;Bin3 _Phormidium&nbsp;nigroviride_ | C5&nbsp; Bin3 _Phormidium&nbsp;nigroviride_ | P1 _Massilia&nbsp;aurea_ | P2 _Janthinobacterium&nbsp;aestuarii_ | A3 _Streptomyces&nbsp;venezuelae_
---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- 
Geosmin (geosmin synthase) | - | **PBBIBEND_00354 Germacradienol/geosmin&nbsp;synthase** | **JFIELPJI_05312 Germacradienol/geosmin&nbsp;synthase** | **PDMAKKBE_00359 Germacradienol/geosmin&nbsp;synthase** | - | - | NKOHJOIO_00838&nbsp;Germacradienol/geosmin&nbsp;synthase NKOHJOIO_01109&nbsp;Germacradienol/geosmin&nbsp;synthase NKOHJOIO_069329&nbsp;hypothetical&nbsp;protein
2-MIB (2-MIB synthase) | - | PBBIBEND_00354 Germacradienol/geosmin&nbsp;synthase | JFIELPJI_05312 Germacradienol/geosmin&nbsp;synthase | PDMAKKBE_00359 Germacradienol/geosmin&nbsp;synthase | - | **Not found** | **NKOHJOIO_00838&nbsp;Germacradienol/geosmin&nbsp;synthase NKOHJOIO_01109&nbsp;Germacradienol/geosmin&nbsp;synthase NKOHJOIO_069329&nbsp;hypothetical&nbsp;protein**
beta-cyclocitral & beta-ionone (carotenoid&nbsp;cleavage&nbsp;dioxygenase1)| **NPBPOGNA_00278 hypothetical&nbsp;protein** | PBBIBEND_03032&nbsp;Apocarotenoid15,15'oxygenase PBBIBEND_02667&nbsp;Apocarotenoid15,15'oxygenase | JFIELPJI_00123&nbsp;Apocarotenoid15,15'oxygenase JFIELPJI_02995&nbsp;Apocarotenoid15,15'oxygenase | PDMAKKBE_03039&nbsp;Apocarotenoid15,15'oxygenase PDMAKKBE_02672&nbsp;Apocarotenoid15,15'oxygenase | **Not found** | - | NKOHJOIO_07584&nbsp;Carotenoid&nbsp;cleavage&nbsp;oxygenase NKOHJOIO_07364&nbsp;Carotenoid&nbsp;cleavage&nbsp;oxygenase

* geoA genes were also hit with 2-MIB synthase due to shared terpene cyclase domain.
* Carotenoid-15,15′-oxygenase genes were hit by CCD1 BLAST queries due to carotenoid oxygenase domains.
