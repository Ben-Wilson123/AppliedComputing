# HDS Computing — Lab 2

## Overview

This lab explores computational analysis of gene expression data using R and Python (in the form of R Markdown and Jupyter Notebooks). The analysis uses the GSE52778 gene expression dataset from the NCBI Gene Expression Omnibus (GEO) to practice data manipulation, visualization, and reproducible computational workflows. This was chosen from the HDS Source.md file.

## Dataset

The dataset used in the R analysis is:

* **GEO accession:** GSE52778
* **Data type:** FPKM gene expression measurements
* **Source:** NCBI Gene Expression Omnibus (GEO)
* **File:** `GSE52778_FPKM.txt.gz`

The compressed dataset is excluded from version control through the repository `.gitignore`.

## R Analysis

The R portion of the lab uses `Lab2R.Rmd` to:

1. Import the GSE52778 FPKM expression matrix.
2. Examine and manipulate the gene expression data.
3. Identify the 10 genes with the highest FPKM values in the `Dex` sample.
4. Visualize the top 10 genes using `ggplot2`.
5. Interpret the resulting expression pattern.

The resulting analysis is documented in `Lab2R.pdf`.

## Python Analysis

The Python portion of the lab uses `Lab2Python.ipynb` to perform computational analysis and visualization using Python with the same dataset, attempting to also achieve the same results as the R script.

The completed notebook is also provided as a PDF: `Lab2Python.pdf`

## Lab Write-Up

As part of the graduate addendum, we were to use both R and Python. After, we were to compare the ease and trustworthiness of the results in both programs. The results can be found in: `Lab2WriteUp.ipynb`

## Environment and Reproducibility

The hds-computing environment was set up in Lab 1. Any alterations made were solely to install more packages such as matplotlib. To run the Jupyter Notebook, click "Run All" after selecting the HDS-computing kernel. To run the R Markdown File, click the three dots in the top right, select "R: Knit", and then select the desired format (for example, Knit.rmd to PDF).

## Files

```text
Lab 2/
├── Lab2Python.ipynb
├── Lab2Python.pdf
├── Lab2R.pdf
├── Lab2R.Rmd
├── Lab2WriteUp.ipynb
└── GSE52778_FPKM.txt.gz
```
