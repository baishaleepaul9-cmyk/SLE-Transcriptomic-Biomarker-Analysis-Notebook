# SLE Transcriptomic Biomarker Analysis Notebook

This repository contains the Google Colab/Jupyter notebook used for the transcriptomic analysis and diagnostic biomarker development for systemic lupus erythematosus (SLE).

## Notebook

**`FINAL_Manuscript_file (7).ipynb`**

The notebook contains the complete computational workflow, including data preprocessing, biomarker selection, diagnostic model development, external validation, and severity-associated gene analysis.

## Datasets Used

The notebook uses publicly available gene-expression datasets from the Gene Expression Omnibus (GEO):

* **GSE65391** — primary discovery/development dataset used for diagnostic model development.
* **GSE81622** — external validation dataset.
* **GSE49454** — external validation dataset.
* **GSE88884** — used for independent severity/statistical analysis of the overlapping genes IFI27, EPSTI1, and ZBP1.

## Running the Notebook

The notebook was developed and executed in **Google Colab**.

1. Download the `.ipynb` notebook.
2. Open it using Google Colab.
3. Connect your Google Drive when prompted.
4. Ensure the required datasets and checkpoint files are available in the Google Drive locations specified in the notebook.
5. Run the cells sequentially or select **Runtime → Run all**.

## Google Drive

The notebook uses Google Drive to store and access datasets, intermediate files, model files, checkpoints, and generated results.

When running the notebook under a different Google account, the required files must be available in the corresponding Google Drive locations.

## Analysis Included

The notebook performs:

* Gene-expression data preprocessing
* Probe-to-gene mapping and expression processing
* Diagnostic biomarker selection
* Diagnostic model development
* Model evaluation
* External validation using GSE81622 and GSE49454
* Severity-associated biomarker analysis using GSE88884
* Statistical testing of selected overlapping genes
* Generation and saving of analysis outputs and figures

## Environment

The notebook is intended for:

* **Google Colab**
* **Python 3**
* Google Drive

The notebook may require additional Python packages that are installed or imported within the notebook itself.

## Reproducibility

To reproduce the analysis, users should obtain the required GEO datasets and provide the required input and checkpoint files in the Google Drive locations expected by the notebook.

The notebook should be executed in Google Colab because parts of the workflow depend on Google Colab and Google Drive functionality.
