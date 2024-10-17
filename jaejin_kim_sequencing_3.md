# gDNA sequencing summary for Prof. Jae-Jin Kim

gDNA sequencing was performed with Oxford Nanopore MinION platform.

* Library preparation, sequencing: Chungmin Kim
* Genome assembly, QC: Bogun Kim, Chungmin Kim

## Sequencing summary

Statistics | PDY3 | PDY4
---- | ---- | ----
Total number of reads (k) | 26.1 | 282.7
Total number of bases (Mbp) | 88.9 | 1311.2
Mean read length (bp) | 2,848 | 3208.6
Mean read quality score | 14.2 | 13.8

## Assembly summary

* Reads with quality score over threshold value were filtered to generate genome with high completeness.
* Reads were assembled with [Flye genome assembler](https://github.com/fenderglass/Flye) v2.9.5 with `--nano-hq --iterations 2` parameters.
* [Medaka](https://github.com/nanoporetech/medaka) v1.7.2 was used to correct errors in the draft genome assembly for PDY4.
* Genome completeness assession with [checkM](https://github.com/Ecogenomics/CheckM) v1.2.3 or [BUSCO](https://busco.ezlab.org/) v5.7.1.

Statistics | PDY3 | PDY4
---- | ---- | ----
Total assembly length (bp) | 5,520,799 | 8,363,733
Number of contigs | 2 | 5
Contig N50 (bp) | 5,497,843 | 7,928,270
Contig L50 | 1 | 1
GC ratio (%) | 66.6 | 72
Genome coverage | 15x | 50x
Genome completeness (%) | 98.9 | 99.7

## 16S rRNA sequence based species evaluation

* 16S rRNA sequence was identified from the genome sequence using [barrnap](https://github.com/tseemann/barrnap) v0.9 with default parameters.
* Identified 16S rRNA sequence aligned against NCBI 16S rRNA database with NCBI [web-BLAST](https://blast.ncbi.nlm.nih.gov/Blast.cgi)
* Average nucleotide identity was calculated using [fastANI](https://github.com/ParBLiSS/FastANI) with 16s rRNA top-matched genome.

### PDY3

* Alignment with 16S rRNA sequence of _Mycolicibacterium neoaurum_ showed 100% identity and genome ANI was 99.08%.

### PDY4

* Alignment with 16S rRNA sequence of _Streptomyces fungicidicus_ showed and 100% genome ANI was 99%.
