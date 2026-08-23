# SLE Transcriptomic Biomarker Analysis

This repository contains the Google Colab/Jupyter notebook used for the
transcriptomic analysis and diagnostic biomarker development for systemic
lupus erythematosus (SLE).

## Contents

- `FINAL_Manuscript_file (7).ipynb` — complete analysis notebook
- Required CSV input files used by the notebook

## Datasets

The analysis uses publicly available gene-expression datasets from the
NCBI Gene Expression Omnibus (GEO):

- **GSE65391** — primary discovery/development cohort used for diagnostic
  biomarker development.
- **GSE81622** — external validation cohort.
- **GSE49454** — external validation cohort.
- **GSE88884** — used for independent statistical and severity-associated
  analysis of the overlapping biomarkers IFI27, EPSTI1, and ZBP1.

## Required Files

The following files are required by the notebook for the archived analysis
and should be available in the working data directory:

- `GSE65391_final_13gene_development_matrix.csv`
- `GSE81622_13gene_input.csv`
- `GSE49454_final_13gene_input.csv`
- `GSE88884_severity_phenotype.csv`

Other intermediate files, models, checkpoints, figures, and statistical
results are generated during execution of the notebook.

## Running the Notebook

The notebook was developed and executed using **Google Colab**.

### Steps

1. Download or clone this repository.
2. Open `FINAL_Manuscript_file (7).ipynb` in Google Colab.
3. Upload or make the required CSV files available in the locations
   expected by the notebook.
4. Connect Google Drive when prompted by the notebook.
5. Run the notebook sequentially, or use **Runtime → Run all**.

## Analysis Workflow

The notebook includes the following major analyses:

- Transcriptomic data preprocessing
- Gene-level expression processing
- Diagnostic biomarker selection
- Development of the final diagnostic model
- Evaluation of diagnostic performance
- External validation using GSE81622 and GSE49454
- Identification of overlapping biomarkers
- Severity-associated analysis using GSE88884
- Statistical testing of selected biomarkers
- Generation of analysis results and figures

## Final Diagnostic Biomarker Panel

The final diagnostic workflow uses a 13-gene biomarker panel:

- IFI27
- RPL5
- ZBP1
- IFITM1
- EPSTI1
- EBI2
- FCER1A
- GADD45A
- TNFSF13B
- IFIT2
- OSBPL10
- SCRN1
- TNFAIP6

## GSE88884 Statistical Analysis

The GSE88884 analysis evaluates the overlapping biomarkers:

- IFI27
- EPSTI1
- ZBP1

The analysis includes associations with disease severity and statistical
comparisons between severity groups.

## Reproducibility

The notebook contains the computational workflow used for the reported
analysis. Intermediate files, models, checkpoints, figures, and statistical
results are generated and/or saved during execution.

The notebook was designed for execution in Google Colab and uses Google
Drive for file storage and intermediate outputs.

Users reproducing the analysis should ensure that the required input CSV
files are available before running the relevant notebook sections.

## Environment

- Google Colab
- Python 3
- Jupyter Notebook

Python packages required by the notebook are imported and/or installed
within the notebook where applicable.
