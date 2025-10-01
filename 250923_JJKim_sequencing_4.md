# gDNA sequencing summary for Prof. Jae-Jin Kim

gDNA sequencing was performed with Oxford Nanopore MinION platform.

* Library preparation, sequencing: Chungmin Kim, Kihyun Nam
* Genome assembly, QC: Chungmin Kim

## Sequencing summary

Statistics | YJAN24 | YJAN111 | YJAN112
---- | ---- | ---- | ----
Total number of reads (k) | 221 | 252 | 245
Total number of bases (Mbp) | 337 | 388 | 386
Mean read length (bp) | 1,525 | 1,543 | 1,575
Mean read quality score | 15.8 | 17.2 | 17.0

## Assembly summary

* For YJAN24, reads were filtered by quality and length threshold to generate genome with high completeness.
* Reads were assembled with [Flye genome assembler](https://github.com/fenderglass/Flye) v2.9.5 with `--nano-hq --iterations 2` parameters.
* Genome completeness were assessed with [checkM](https://github.com/Ecogenomics/CheckM) v1.2.4


Statistics | YJAN24 | YJAN111 | YJAN112
---- | ---- | ---- | ----
Total assembly length (bp) | 2,985,980 | 2,237,711 | 2,216,764
Number of contigs | 1 | 1 | 1
Genome coverage | 56x | 186x | 185x
Circular | N (repeat) | Y | Y
Genome completeness (%) | 99.2 | 99.6 | 99.6

## 16S rRNA sequence and ANI based species evaluation

* 16S rRNA sequence was identified from the genome sequence using [barrnap](https://github.com/tseemann/barrnap) v0.9 with default parameters.
* Identified 16S rRNA sequence aligned against NCBI rRNA/ITS database or standard database with NCBI [web-BLAST](https://blast.ncbi.nlm.nih.gov/Blast.cgi)
* Average nucleotide identity was calculated using [fastANI](https://github.com/ParBLiSS/FastANI) to reference genomes of 16s rRNA top-matched species-containing genus.
* For genomes with low ANI to reference genomes, GTDBtk was used for idenfication.

### YJAN24
* Alignment with 16S rRNA sequence of _Sulfonitrofixus jiaomeiensis_ showed 97% identity and genome ANI was 79%.
* No closest genome was found by GTDBtk.

### YJAN111
* Alignment with 16S rRNA sequence of _Sulfurovum xiamenensis_ showed 95% identity and genome ANI was 96%.

### YJAN112
* Alignment with 16S rRNA sequence of _Sulfurovum xiamenensis_ showed 95% identity and genome ANI was 87%.
* [GCF_019972115 (_Sulfurovum_ sp. TSL6)](https://www.ncbi.nlm.nih.gov/datasets/genome/GCF_019972115.1/) was found as closest genome by GTDBtk with ANI of 98.51%.
