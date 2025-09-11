# Internship Research Project

[![Python](https://img.shields.io/badge/python-3.10-blue.svg)](#)

> This project utilizes Jurkat cell lines as a model to compare dynamic proteomic changes under TCR stimulation versus dual TCR+PD1 stimulation conditions using large-scale mass spectrometry data. Through data preprocessing, normalization, statistical analysis, and downstream pathway enrichment, we explore PD1 activation's regulatory role in immune signaling, identify potential key molecules and pathways, and provide data-driven insights for immunotherapy-related research.
> 
> **Whole-Proteome Analysis**, **Mass Spectrometry Data**, **Jurkat Cell Line**, **T Cell Receptor (TCR)**, **Programmed Cell Death Protein 1 (PD1)**, **Data Preprocessing and Normalization**, **Differential Protein Expression Analysis**, **Pathway Enrichment Analysis**, **Protein Interaction Network Analysis**, **Statistical and Machine Learning Methods**, **Immune Checkpoint Regulation**, **Signal Transduction Mechanisms**, **Immunotherapy Biomarkers**, **Cancer Immunology**, **Precision Medicine**

---

## Project Object

This project aims to analyze whole-proteome mass spectrometry data generated from a Jurkat T cell model to investigate the immunoregulatory role of the PD-1 checkpoint receptor.

Specifically, the objective is to:
- Compare T cell signaling under two conditions:
    - Control: TCR receptor stimulation alone
    - Experimental: TCR + PD-1 receptor co-stimulation across multiple timepoints
- Identify differentially expressed proteins between the two conditions
- Reveal signaling pathways potentially involved in PD-1–mediated modulation of TCR signaling

## Quick Start

### Project Directory Structure

The complete directory structure is as follows:

```bash
internship_reaserch_project/
        ├─ project_work.ipynb                           # The code part of the project
        ├─ report/
        │  ├─ figures/                                  # Images embedded in reports
        │  ├─ neurips_2023.sty                          # LaTeX template style file
        │  ├─ internship_research_project_report.tex    # The source file of the report
        │  └─ internship_research_project_report.pdf    # The project report
        ├─ LICENSE                                      # This project employs a custom licence; for details, see LICENCE
        └─ README.md
```

### Create Running Environment

I recommend using Conda/Anaconda together with Visual Studio Code as the IDE for running or debugging the Jupyter Notebook code. I haven't tested other environments, but if you are familiar with them, you may also set up and run the notebook by referring to the instructions. Below, I demonstrate how to set up the environment using my recommended configuration:

To reproduce the project results, you first need to have a Conda environment installed (if not, see the [Conda documentation](https://docs.conda.io/projects/conda/en/stable/) for installation instructions). Then, run the following shell commands to create an environment suitable for executing the Jupyter Notebook code (I also included these commands in the notebook for reference):

```bash
(base) user@device internship_reaserch_project % conda create -n irp-lab-env python=3.10 -y
(base) user@device internship_reaserch_project % conda activate irp-lab-env
(irp-lab-env) user@device internship_reaserch_project % pip install numpy pandas matplotlib scipy statsmodels gseapy networkx scikit-learn seaborn
```

After creating the environment, simply open the Jupyter Notebook in Visual Studio Code and select the Python environment `irp-lab-env` that you just created as the interpreter. You can then execute the notebook code cell by cell.
