# Lab 3 — Regex-Based Data Cleaning

## Overview

This lab focuses on cleaning and structuring messy input files with Regex and AI-assisted cleaning techniques, along with an addendum to create a sample x features x metadata table. The input files were:

* A messy sample metadata CSV file
* A messy DNA sequence FASTA file

The outputs produced using regex expressions are compared with corresponding AI-cleaned outputs in a write-up file. 

## Project Structure

```text
Lab 3/
├── README.md
├── AI_USAGE.md
├── data/
│   ├── messy_samples.csv
│   ├── messy_sequences.fasta
│   ├── cleaned_samples_AI.csv
│   ├── cleaned_samples_regex.csv
│   ├── cleaned_sequences_AI.fasta
│   └── cleaned_sequences_regex.fasta
│
├── notebooks/
│   ├── Regex_CSV.ipynb
│   ├── Regex_FASTA.ipynb
│   └── WriteUp.ipynb
│
└── scripts/
    └── generate_data.py
```

## Notebooks

### `Regex_CSV.ipynb`

Contains the reegex workflow for cleaning the messy sample CSV as well as the graduate addendum.

### `Regex_FASTA.ipynb`

Contains the regex workflow for parsing and cleaning the messy FASTA headers.

### `WriteUp.ipynb`

Contains the comparison of the AI and regex cleaning approaches.

## Running the Project

From the `Lab 3` directory, open the notebooks in VS Code or Jupyter. Click "Run All" to run all individual code blocks. The inputs are already in the data folder, so there should not be any extra work required.

Because the notebooks are stored in the `notebooks/` directory and the data is stored in `data/`, data paths use the following format:

```python
"../data/messy_samples.csv"
```

Cleaned outputs should also be written to the `data/` directory.

## Reproducibility

The original messy files are retained separately from the cleaned outputs so that the cleaning process can be reproduced and the AI and regex approaches can be compared without modifying the original data as shown in WriteUp.ipynb.