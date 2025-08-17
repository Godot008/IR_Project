# Internship Research Project

[![Python](https://img.shields.io/badge/python-3.10-blue.svg)](#)

> This is an individual internship research project that I completed based on the data and requirements provided by my supervisor during the summer trimester at UCD.
> 
> **Proteomics**, **PD-1 signaling**, **TCR pathway**, **Differential expression analysis**, **Differential expression analysis**, **Clustering analysis**, **Protein–protein interaction (PPI) network**, **Immune checkpoint inhibitors (ICI)**

---

## Quick Start

### Project Directory Structure

The complete directory structure is as follows:

```bash
internship_reaserch_project/
        ├─ project_work.ipynb                           # the code part of the project
        ├─ report/
        │  ├─ figures/                                  # images embedded in reports
        │  ├─ neurips_2023.sty                          # LaTeX template style file
        │  ├─ internship_research_project_report.tex    # the source file of the report
        │  └─ internship_research_project_report.pdf    # the project report
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
