# gDNA sequencing summary for 한강통합물환경센터

gDNA sequencing was performed with Oxford Nanopore MinION platform. Sequencing and analysis done by Chungmin Kim.

* Library preparation: SQK-RBK114.24
* Sequencing: FLO-MIN114 in Mk1B
* Basecalling: Dorado (v2.1.2) with dna_r10.4.1_e8.2_400bps_sup@v5.2.0

## Workflow

Read QC: SeqKit (v2.13.0)
De novo Assembly: nanoMDBG (v1.4)
Binning & Refinement: MetaBAT2 (v2.18), SemiBin2 (v2.4.1) & Binette (v1.2.1)
Quality Assessment: CheckM2 (v1.1.0)
Taxonomic Classification: GTDB-Tk (v2.5.0, Release 226)

## Yield summary

| Statistics | C06 | C07 | C08 | C09 | C10 | C11 | C12 | C13 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Total number of reads (k) | 427 | 748 | 585 | 858 | 521 | 838 | 662 | 287 |
| Total number of bases (Mbp) | 858 | 1,401 | 1,224 | 2,181 | 1,056 | 1,592 | 1,630 | 597 |
| Read N50 (bp) | 4,348 | 3,777 | 4,408 | 5,505 | 4,447 | 3,925 | 5,386 | 4,388 |
| Median read quality score | 19.5 | 20.2 | 19.4 | 21.1 | 19.5 | 19.5 | 19.0 | 20.0 |

| Statistics | C14 | C15 | C16 | C17 | C18 | C19 | C20 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Total number of reads (k) | 893 | 364 | 518 | 829 | 339 | 273 | 529 |
| Total number of bases (Mbp) | 1,855 | 570 | 1,000 | 1,898 | 930 | 953 | 1,636 |
| Read N50 (bp) | 4,129 | 2,947 | 4,257 | 5,248 | 5,826 | 7,879 | 6,632 |
| Median read quality score | 19.4 | 21.1 | 18.9 | 19.3 | 19.6 | 19.4 | 19.4 |


## Assembly summary

Statistics | C06 | C07 | C08 | C09 | C10 | C11 | C12 | C13
---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ----
Number of contigs | 1,444 | 861 | 161 | 554 | 312 | 540 | 99 | 749
Total assembly length (kbp) | 47,167 | 46,837 | 24,011 | 57,104 | 26,105 | 32,597 | 13,217 | 29,759
Contig N50 (kbp) | 51 | 263 | 3,222 | 3,242 | 3,241 | 134 | 3,994 | 3,241
Largest contig (kbp) | 6,587 | 6,593 | 6,609 | 6,891 | 6,588 | 6,587 | 6,593 | 6,596
 
Statistics | C14 | C15 | C16 | C17 | C18 | C19 | C20
---- | ---- | ---- | ---- | ---- | ---- | ---- | ----
Number of contigs | 23 | 777 | 101 | 91 | 529 | 480 | 54
Total assembly length (kbp) | 11,535 | 28,955 | 13,525 | 16,112 | 37,266 | 36,106 | 26,657
Contig N50 (kbp) | 6,598 | 201 | 3,994 | 3,994 | 706 | 1,002 | 3,994
Largest contig (kbp) | 6,598 | 4,437 | 6,586 | 6,603 | 6,596 | 6,603 | 6,609
 
## Binning summary
 
* MAG quality
  * High quality (Completeness > 90% and Contamination < 5%)
  * Medium quality (Completeness ≥ 50% and Contamination < 10%)
  * Low quality (Completeness < 50% or Contamination ≥ 10%)

Statistics | C06 | C07 | C08 | C09 | C10 | C11 | C12 | C13
---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ----
No. of HQ MAG | 4 | 8 | 5 | 9 | 5 | 6 | 2 | 3
No. of MQ MAG | 6 | 3 | 1 | 2 | 1 | 1 | 1 | 3
No. of LQ MAG | 0 | 0 | 0 | 1 | 0 | 0 | 0 | 0
Total MAGs | 10 | 11 | 6 | 12 | 6 | 7 | 3 | 6

Statistics | C14 | C15 | C16 | C17 | C18 | C19 | C20 | Total
---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ----
No. of HQ MAG | 2 | 3 | 2 | 3 | 6 | 4 | 6 | 68
No. of MQ MAG | 0 | 3 | 1 | 0 | 1 | 3 | 0 | 26
No. of LQ MAG | 0 | 0 | 0 | 0 | 2 | 1 | 0 | 4
Total MAGs | 2 | 6 | 3 | 3 | 9 | 8 | 6 | 98
 
## Geosmine-producing _Phormidium_ (_Microcoleus_)
  
* _Phormidium_ and its geoA genes was detected in all samples.
* All _Phormidium_ have 99.9% genome ANI except for one from C09 sample (85% with C09 _Phormidium_).
* Likewise, geoA gene sequence was 100% identical except for _Phormidium_ C09.

Statistics | C06 | C07 | C08 | C09 | C10 | C11 | C12 | C13
---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ----
Bin ID | binette_bin2 | binette_bin5 | binette_bin3 | binette_bin3 | binette_bin2 | binette_bin5 | binette_bin2 | binette_bin3
Species | _Microcoleus_ sp015207505 | _Microcoleus_ sp015207505 | _Microcoleus_ sp015207505 | **_Microcoleus_ sp036701635** | _Microcoleus_ sp015207505 | _Microcoleus_ sp015207505 | _Microcoleus_ sp015207505 | _Microcoleus_ sp015207505
Completeness (%) | 100.0 | 99.99 | 99.98 | 100.0 | 99.98 | 99.93 | 99.99 | 99.88
Contamination (%) | 0.17 | 0.02 | 0.01 | 0.00 | 0.00 | 0.00 | 0.12 | 0.10
Genome size (bp) | 6,586,680 | 6,592,661 | 6,608,769 | 6,891,276 | 6,587,712 | 6,586,509 | 6,593,333 | 6,596,173

Statistics | C14 | C15 | C16 | C17 | C18 | C19 | C20
---- | ---- | ---- | ---- | ---- | ---- | ---- | ----
Bin ID | binette_bin2 | binette_bin3 | binette_bin2 | binette_bin3 | binette_bin2 | binette_bin2 | binette_bin4
Species | _Microcoleus_ sp015207505 | _Microcoleus_ sp015207505 | _Microcoleus_ sp015207505 | _Microcoleus_ sp015207505 | _Microcoleus_ sp015207505 | _Microcoleus_ sp015207505 | _Microcoleus_ sp015207505
Completeness (%) | 99.99 | 99.57 | 99.99 | 99.98 | 99.99 | 99.97 | 99.97
Contamination (%) | 0.00 | 0.32 | 0.53 | 0.00 | 0.00 | 0.00 | 0.00
Genome size (bp) | 6,597,573 | 6,435,187 | 6,586,262 | 6,602,742 | 6,595,926 | 6,603,111 | 6,608,519

<br>

## ANI (Whole genome & geoA gene)

<img src="https://github.com/user-attachments/assets/8dd4de91-76e3-4b04-b8d2-2060793655ee" width="400">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="https://github.com/user-attachments/assets/4db46ca0-b091-42cf-a310-b98e8b9d5e7f" width="400">
