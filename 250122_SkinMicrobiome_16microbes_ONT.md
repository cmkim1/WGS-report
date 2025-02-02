# WGS summary of 16 microbes isolated from skin

Microbes were isolated from Chungmin Kim, Kihyeon Nam, Minkoo Jeong.  
gDNA was extracted with GeneAll Exgene Cell SV kit.  
gDNA sequencing was performed with Oxford Nanopore MinION platform.  

* DNA extraction: Chungmin Kim, Kihyeon Nam, Minkoo Jeong
* Library preparation, sequencing: Chungmin Kim
* Genome assembly, QC: Chungmin Kim

## Sequencing summary

Metrics | CMK7 | CMK11 | CMK15 | CMK28 | NKH7 | NK14 | NKH16 | MKJ2
---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ----
Total number of reads (k) | 512.6 |874.1 | 637.6 | 340.8 | 269.3 | 235.6 | 422.9 | 28.9
Total number of bases (Mbp) | 2019.7 |2335.7 | 1847.9 | 1648.7 | 1149.3 | 1300.6 | 2837.3 | 50
Read N50 (bp) | 9085 |5308 | 6500 | 9882 | 10396 | 10063 | 12417 | 10582
Mean read quality score | 15.9 |16.1 | 16 | 15.8 | 15.9 | 14.3 | 16 | 8.6

Metrics | MKJ4 | MKJ5 | MKJ8 | MKJ11 | MKJ12 | MKJ25 | NKH8 | CSBL15
---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ----
Total number of reads (k) | 60.2 | 185.8 | 47.3 | 135 | 52.5 | 142.4 | 63.7 | 288.8
Total number of bases (Mbp) | 229.7 | 474.9 | 70.9 | 228.1 | 255.3 | 445.8 | 229.4 | 1196
Read N50 (bp) | 13000 | 6730 | 9358 | 6349 | 13490 | 8101 | 14557 | 8188
Mean read quality score | 10.6 | 15.3 | 8.8 | 15.1 | 12.2 | 14 | 9.9 | 16

## Assembly summary

* Reads with quality score and length over threshold were filtered with [Nanofilt](https://github.com/wdecoster/nanofilt) (Galaxy Version 0.1.0)
* Reads were assembled with [Flye genome assembler](https://github.com/fenderglass/Flye) Galaxy Version 2.9.5+galaxy1 with default parameters.


Metrics | CMK7 | CMK11 | CMK15 | CMK28 | NKH7 | NK14 | NKH16 | MKJ2
---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ----
Total assembly length (bp) | 2,504,345 | 2,238,962 | 2,264,338 | 2,198,468 | 2,436,555 | 2,483,457 | 2,504,346 | 2,520,519
Number of contigs | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1
Contig N50 (bp) | 2,504,345 | 2,238,962 | 2,264,338 | 2,198,468 | 2,436,555 | 2,483,457 | 2,504,346 | 2,520,519
Contig L50 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1
GC ratio (%) | 0.32 | 0.32 | 0.32 | 0.33 | 0.32 | 0.32 | 0.27 | 0.73
Genome coverage | 177 | 30 | 26 | 28 | 77 | 73 | 67 | 13
Genome completeness (%) | 99.81 | 99.38 | 99.38 | 99.81 | 99.81 | 99.81 | 99.81 | 98.7

Metrics | MKJ4 | MKJ5 | MKJ8 | MKJ11 | MKJ12 | MKJ25 | NKH8 | CSBL15
---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ----
Total assembly length (bp) | 2,517,864 | 2,246,689 | 2,511,238 | 4,252,383 | 5,361,359 | 2,499,638 | 5,137,574 | 2,404,989
Number of contigs | 1 | 1 | 1 | 1 | 3 | 1 | 4 | 1
Contig N50 (bp) | 2,517,864 | 2,246,689 | 2,511,238 | 4,252,383 | 5,361,359 | 2,499,638 | 5,137,574 | 2,404,989
Contig L50 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1
GC ratio (%) | 0.73 | 0.32 | 0.73 | 0.46 | 0.56 | 0.44 | 0.71 | 0.32
Genome coverage | 20 | 67 | 19 | 44 | 40 | 31 | 39 | 99
Genome completeness (%) | 98.7 | 99.38 | 98.7 | 98.96 | 99.62 | 99.71 | 100 | 99.38


## Species identification
* Average nucleotide identity was calculated using [fastANI](https://github.com/ParBLiSS/FastANI) with reference genomes in the same genus.

Metrics | CMK7 | CMK11 | CMK15 | CMK28 | NKH7 | NK14 | NKH16 | MKJ2
---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ----
Genus | _Staphylococcus_ | _Staphylococcus_ | _Staphylococcus_ | _Staphylococcus_ | _Staphylococcus_ | _Staphylococcus_ | _Staphylococcus_ | _Micrococcus_
Species | _epidermidis_ | _hominis_ | _hominis_ | _capitis_ | _epidermidis_ | _epidermidis_ | _epidermidis_ | _yunnanensis_
ANI | 99.39 | 98.97 | 97.35 | 96.65 | 99.49 | 99.89 | 99.9 | 97.97

Metrics | MKJ4 | MKJ5 | MKJ8 | MKJ11 | MKJ12 | MKJ25 | NKH8 | CSBL15
---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ----
Genus | _Micrococcus_ | _Staphylococcus_ | _Micrococcus_ | _Bacillus_ | _Pseudomonas_ | _Moraxella_ | _Roseomonas_ | _Staphylococcus_
Species | _yunnanensis_ | _hominis_ | _yunnanensis_ | _licheniformis_ | _zeshuii_ | _osloensis_ | _mucosa_ | _hominis_
ANI | 97.93 | 97.31 | 97.89 | 99.69 | 99.85 | 96.62 | 98.73 | 97.27
<br>

* Pairwise ANI between Staphylococci  

<img src = "https://github.com/user-attachments/assets/da31f8b2-4f81-4cd4-b944-06a3aae8515d" width="60%" height="60%">
