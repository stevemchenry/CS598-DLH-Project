# Medical-Record-Linkage-Ensemble
Medical-Record-Linkage-Ensemble
This repository contains the full code of the paper "Statistical supervised meta-ensemble algorithm for data linkage", published in Journal of Biomedical Informatics. 

Authors: 
Kha Vo <kha.vo@unsw.edu.au>
Jitendra Jonnagaddala <jitendra.jonnagaddala@unsw.edu.au>
Siaw-Teng Liaw <siaw@unsw.edu.au>

+ All of the code in this repository used Python 3.6 or higher with these prerequisite packages: `numpy`, `pandas`, `sklearn`, and `recordlinkage`. For installing aa missing package, use command `pip install package-name` in a terminal (i.e., cmd in Windows, or Terminal in MacOS).

0a. Prepare the cleaned datasets for Scheme A, which are stored in two files `febrl3_UNSW.csv` and `febrl3_UNSW.csv`. To reproduce those two files, use Python Notebook (i.e., Jupyter Notebook of Anaconda3 distribution) to run `Rectify_Febrl_Datasets.ipynb`.

0b. Prepare the synthetic ePBRN-error-simulated datasets for Scheme B, which are stored in two files `ePBRN_D_dup.csv` and `ePBRN_F_dup.csv`. The original FEBRL dataset (all original, no duplicate) is contained in 2 files: `/ePBRN_Datasets/ePBRN_D_original.csv` and `/ePBRN_Datasets/ePBRN_F_original.csv`. To reproduce `ePBRN_D_dup.csv` and `ePBRN_F_dup.csv`, run `Error_Generator.ipynb`. In the first cell of the notebook, change variable `inputfile` to either `ePBRN_D_original` or `ePBRN_F_original`, which is respectively corresponding to variable `outputfile` of `ePBRN_D_dup` or `ePBRN_F_dup`. 

1. Reproduce results for Scheme A in the paper by running `FEBRL_UNSW_Linkage.ipynb`.

2. Reproduce results for Scheme B in the paper by running `ePBRN_UNSW_Linkage.ipynb`.

3. The plots in the paper can be reproduced by running `Plots.ipynb`.
