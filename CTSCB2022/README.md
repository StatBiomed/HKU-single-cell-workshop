# Bioinformatics Rotation Training

This page is designed for 2022-intake students in 
[CTSCB](https://www.hkstemcell.hk) to get preliminary training in 
bioinformatics and analytics skills in single-cell data.


The rotation training is one day per week, across 8 weeks. Besides the training 
day, there will be a few hours of self-reading & practice to further enhance the
skills.

## Week 1: Basic programming with R
* Read the 1h course material on 
  [Quantitative_Skills_I](https://github.com/StatBiomed/GenomeScienceCourse/blob/master/quant_skills/Quantitative_Skills_I_YHuang.pdf)
* Finish the exercise in [slide P22](https://github.com/StatBiomed/GenomeScienceCourse/blob/master/quant_skills/Quantitative_Skills_I_YHuang.pdf)
* Read and try the [materials designed by Joshua Ho & lab](https://holab-hku.github.io/R-workshop/) chapters 1 to 7.
* Other resources include [Computational Genomics with R](https://compgenomr.github.io/book/Rintro.html)


## Week 2: Analysis of bulk RNA-Seq
* read my lecture notes 
  [Transcriptomics I & II](https://github.com/StatBiomed/GenomeScienceCourse/tree/master/transcriptomics)
* finish the [Assignment 1](https://github.com/StatBiomed/GenomeScienceCourse/tree/master/assignments)
* Read and try the [materials designed by Joshua Ho & lab](https://holab-hku.github.io/R-workshop/) chapter 8.
* Other resources include [Computational Genomics with R](https://compgenomr.github.io/book/rnaseqanalysis.html) chapter 8.


## Week 3: Single-cell data pre-processing
* Learn Linux Command Lines, see more guidelines on the [Linux page](Linux_learn.md)
* Start to use Center Computing server
<!-- * Alignment and reads counting: [smart-seq data](https://github.com/huangyh09/brie/tree/master/examples/gastrulation) -->
* CellRanger for 10x genomics data: [1K PBMC data](https://www.10xgenomics.com/resources/datasets/1-k-pbm-cs-from-a-healthy-donor-v-3-chemistry-3-standard-3-0-0)
* Read and play with [Workshop materials](https://holab-hku.github.io/Fundamental-scRNA/)


## Week 4: Seurat for single-cell analysis
* Seurat [tutorial with 3K PBMC data](https://satijalab.org/seurat/articles/pbmc3k_tutorial.html)
* Read and play with [Workshop materials](https://holab-hku.github.io/Fundamental-scRNA/) chapter 3
* Try and compare to automatic cell type annotation, e.g, by [CellTypist](https://www.celltypist.org/) and [Azimuth](https://azimuth.hubmapconsortium.org/) (Optional and practically useful)


## Week 5: Cell clustering & annotation
* 10x genomic data, tentatively from the [CARLIN paper](https://www.cell.com/cell/fulltext/S0092-8674(20)30554-7)
* Get the data from [GSE146972](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE146972) and using the processed cell-by-gene count matrices in *h5 format in the **Supplementary file**. You are recommended to start with **EB_FO864_SC_LF_Transcriptome** but you can also try integrating all samples.
* Annotation by markers
* Annotation by automatic prediction


## Week 6: Mitochondrial variants analysis
* Read [MQuad paper](https://www.nature.com/articles/s41467-022-28845-0) 
  on the processing of Kim dataset, 
  [manual](https://github.com/single-cell-genetics/MQuad),
  and the [analysis codes/data on Kim data](https://github.com/aaronkwc/MQuad_paper_reproduced_results/tree/main/kim). 
* Analyse one dataset. Tentatively the Kim data with 121 cells (smart-seq data, one cell per file): 
  [GSE73121](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE73121)
* Read and play with [Workshop materials](https://statbiomed.github.io/SingleCell-Workshop-2021/SNV-analysis.html) chapter 4


## Week 7-8: Group Project
* Sub-group meeting without Dr Huang.
  You are encouraged to define your own project and find your own data sets (as a group; at least one dataset)
* Option 1: hematopoietic data, e.g., [MAESTER data, Fig. 2](https://www.nature.com/articles/s41587-022-01210-8#Fig2), 
  data [GSE182685](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE182685) for **BPDCN712_10x_scRNAseq** and **BPDCN712_10x_MAESTER**
* Option 2: EPSC or Blastoids, e.g.,
  [iBlastoids paper](https://www.nature.com/articles/s41586-021-03372-y)
* Option 3: lung and airway, e.g., 
  [asthma paper](https://www.cell.com/cell-reports/fulltext/S2211-1247(20)30853-6)
  for identifying hybrid cells (between ciliated and secretory)

## Week 9: Presentation
* Tentatively on 15/08 (10am)