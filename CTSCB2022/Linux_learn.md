# Guidelines for learning Linux OS and CLI

## Materials
1. a very good online course from Google (on coursera):
  [OS and power user](https://www.coursera.org/learn/os-power-user). You can audit the course and only read the Linux part and ignore Windows Operating System

2. Dave Child's cheat sheet: [html online version](https://cheatography.com/davechild/cheat-sheets/linux-command-line/)

3. General [guidelines on SBMS server](https://github.com/StatBiomed/sbms-server). There will be one for center server soon.


## What to achieve today
1. Login to server with SSH
   ```sh
   ssh 10.64.246.14

   ssh USER@10.64.246.14
   ssh 10.64.246.14 -l USER
   ```

2. nevigate directory with `cd`, `ls`, `pwd`, `mkdir`
3. read and touch files with `less` and `cat`
4. move, copy and remove files: `mv`, `cp` and `rm`
5. download data with `wget`
6. unzip files with `tar`, `gzip` and `zip`. 
   [Example use `tar`](https://phoenixnap.com/kb/extract-tar-gz-files-linux-command-line)
7. and the more the better (the course above is a great place)


## What to achieve this week
1. Reference and cellranger from 10x genomics (downloaded by Weiyu); [download page](https://support.10xgenomics.com/single-cell-gene-expression/software/downloads/latest)
2. Sequencing data (downloaded by Weiyu): [1K PBMC data](https://www.10xgenomics.com/resources/datasets/1-k-pbm-cs-from-a-healthy-donor-v-3-chemistry-3-standard-3-0-0)
3. Run CellRanger for the above 10x genomics data
4. Explore the technical reports from cellranger

For each of you, only download cell-by-gene count matrix and play with the commandlines above, e.g., `tar`, `mv`:
```bash
wget https://cf.10xgenomics.com/samples/cell-exp/3.0.0/pbmc_1k_v3/pbmc_1k_v3_filtered_feature_bc_matrix.tar.gz
```