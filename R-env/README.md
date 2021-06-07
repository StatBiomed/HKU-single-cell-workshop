# R environment set up

There are multiple ways to set up an R environment and install the needed R
packages for this course on single-cell data analysis.

Here, we introduce one of them to set up the environment with conda.

## 1. Using conda environment

### Step 0: install conda with miniconda or Anaconda

**Note:** You can type ``which conda`` check if you have conda installed. If yes, it will return a path, and you don't need to install conda again - you can skip this step.

If you don't have conda in your system, you can either install [mimiconda](https://docs.conda.io/en/latest/miniconda.html) or [Anaconda](https://docs.anaconda.com/anaconda/install/). Generally, we recommend using *minicoda* for users with limited storage, which gives all you need for this course. On the other hand, Anaconda will contain many other useful tools for programming and analysis.


### Step 1: create conda environment

Once you installed conda on your computer, you can create new and clean environment for this course (or your future use too).

Now you need to use your terminal for the followings. [Please provide guidance on using terminal]

* Add the conda channels (this step may be needed)
  ```bash
  conda config --add channels r
  conda config --add channels conda-forge
  ```

* Create a conda environment with both R 4.1 kernel and Rstudio

  ```bash
  conda create r_env r-essentials==4.1 rstudio==1.1.456
  ```

### Step 2: install R package in R environment

Once you installed conda environment, you can activate it from terminal with the following command line:

```bash
conda activate r_env
```

Then, you can open RStudio or R from terminal by typing ``rstudio`` or ``R``.

* Play with R function
  ```R
  plot(sample(10), sample(10))

  # check session info
  sesionInfo()
  ```

* Install Seurat package
  ```R
  install.packages('Seurat')
  ```


### Step 3: install more packages for the remaining course

* Possibly install ``destiny``
  ```R
  if (!requireNamespace("BiocManager", quietly = TRUE))
      install.packages("BiocManager")
  BiocManager::install("destiny")

  devtools::install_github("theislab/destiny")
  ```


* Install inferCNV and copykat
  ```R
  # install infercnv
  if (!requireNamespace("BiocManager", quietly = TRUE))
      install.packages("BiocManager")
  BiocManager::install("infercnv")

  # install copykat
  devtools::install_github("navinlabcode/copykat")
  ```



<!-- ### Misc

Manually install additional packages via conda
```bash
conda install -c conda-forge r-devtools
conda install -c bioconda r-monocle3==1.0.0
conda install -c conda-forge jags=4.3.0
```

Packages available on conda failed to be installed
```bash
conda install -c bioconductor bioconductor-infercnv==1.6.0
conda install -c bioconductor r-seurat==3.0.2
conda install -c bioconductor bioconductor-destiny==3.4.0
``` 

-->