# SARS-CoV-2-Genomic-Architecture-Analysis


![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![BioPython](https://img.shields.io/badge/BioPython-1.81-green)
![Status](https://img.shields.io/badge/Status-Complete-success)
![License](https://img.shields.io/badge/License-MIT-yellow)

## 🧬 Project Overview

This project implements a computational biology pipeline to analyze the **SARS-CoV-2 reference genome (Accession: NC_045512.2)**. 

Utilizing the **BioPython** ecosystem, the script automates the retrieval of genomic data from the NCBI Nucleotide database, performs statistical composition analysis, and visualizes genomic heterogeneity. The workflow demonstrates a reproducible approach to basic genomic characterization and *in silico* protein translation.

## 🎯 Key Objectives

1.  **Automated Data Ingestion:** Programmatic retrieval of viral sequences using the **NCBI Entrez API**.
2.  **Compositional Metrics:** Calculation of global and local GC content to assess genomic stability.
3.  **Data Visualization:** Implementation of a "Sliding Window" algorithm to map GC heterogeneity across the 29.9kb genome.
4.  **Sequence Translation:** Simulation of the Central Dogma to identify Open Reading Frames (ORFs) within the Spike (S) protein locus.

## 🛠️ Technologies & Libraries

* **Python 3.x**: Core logic.
* **BioPython (`Bio.Entrez`, `Bio.SeqIO`)**: Biological file parsing and API communication.
* **Matplotlib**: Scientific visualization.
* **NumPy**: Numerical operations (implied).
* **Jupyter Notebook**: Interactive development environment.

## 📊 Analysis & Visualization

### 1. Genomic Landscape (GC Content)
The analysis reveals that SARS-CoV-2 is an **AT-rich** genome (Global GC ~38%). However, local variations exist. The plot below utilizes a 300bp sliding window to visualize these fluctuations, which are critical for understanding codon usage bias and evolutionary pressure.

![GC Content Visualization](gc_plot.png)
*(Note: Please ensure `gc_plot.png` is uploaded to your repository for this image to render)*

### 2. Protein Translation
Targeting the Spike protein region (Coordinates: 21,563 - 25,384), the script successfully translated the nucleotide sequence into amino acid residues, identifying potential transmembrane helices based on Leucine content.

## 🚀 Usage

To replicate this analysis:

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/Odariola/covid-genomic-analysis.git](https://github.com/YOUR_USERNAME/covid-genomic-analysis.git)
