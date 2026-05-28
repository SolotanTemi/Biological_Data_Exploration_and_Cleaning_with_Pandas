# Biological Data Exploration and Cleaning with Pandas

## Overview
This project practises essential data manipulation and exploration skills using 
the `bacteria_data` dataset — a collection of 50 *Escherichia coli* isolates with 
antibiotic fitness scores, phenotypic labels, and isolation metadata. The goal is 
to inspect, filter, clean, and summarise biological data using Pandas.

## Dataset
- **Source:** HackBio Internship 2025 Project Collection
- **File:** `bacteria.csv`
- **Shape:** 50 rows × 14 columns
- **Key columns:** `sample_id`, `species`, `Isolation origin`, `Phenotype`, `BSL`,
  `carb_fit`, `cipro_fit`, `genta_fit`, `kan_fit`, `pip_fit`, `labels`

## Tools & Libraries
- Python 3
- Pandas
- Jupyter Notebook

## Project Structure

| Part | Description |
|------|-------------|
| Part 1 | Confirming the dataset — shape and column names |
| Part 2 | Data selection — retrieving rows and columns using `.iloc` and `.loc` |
| Part 3 | Data filtering — subsetting rows based on fitness thresholds |
| Part 4 | Handling missing data — identifying, filling, and dropping NaN values |
| Part 5 | Column renaming — renaming `C1` and `C2` to `UMAP1` and `UMAP2` |
| Part 6 | Sorting — ordering isolates by descending BSL value |
| Part 7 | Grouping analysis — calculating mean and maximum fitness scores by label type |

## Key Findings
- The dataset contains **3 missing values**, all located in the `soln` column
- After filtering for `carb_fit > 0.5`, a meaningful subset of high-fitness isolates is retained
- Grouping by `labels` reveals variation in mean `cipro_fit` and `carb_fit` across bacterial clusters
- Commensal strains (32) outnumber Pathogenic strains (18) in this dataset

## How to Run
1. Clone this repository
2. Open `Biological_Data_Exploration_and_Cleaning_with_Pandas.ipynb` in Jupyter Notebook
3. Run all cells from top to bottom (`Kernel → Restart & Run All`)
