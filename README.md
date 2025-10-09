# Core Resistance Gene Analysis Pipeline

A Python pipeline for identifying and interpreting **core resistance candidate genes** from differential expression datasets, with structural interpretations for actionable insights in drug discovery.

---

## 🧩 Overview

This pipeline:

1. Loads differential expression data (CSV/Excel-derived CSV) for multiple time points.  
2. Cleans and filters genes based on **log2 fold change > 1.5**.  
3. Combines results across time points to identify **core resistance candidates**.  
4. Provides **structural interpretations** and **actionable insights** for top candidates using placeholder sequences.

---

## ⚡ Features

- **Robust Data Cleaning**: Handles whitespace and header inconsistencies.  
- **Candidate Prioritization**: Filters genes with significant log2FC and deduplicates by gene name.  
- **Structural Insights**: Generates preliminary functional interpretations for top candidates (e.g., methyltransferases, RPP13-like proteins).  
- **Actionable Guidance**: Suggests potential targets for drug discovery or synthetic mimetic design.  
- **Output**: Full candidate list saved to CSV and a structural summary printed to console.

---

## 🛠️ Installation

1. Clone this repository

2. Install required dependencies:

pip install pandas

---

## 🗂️ Usage

1. Set the BASE_PATH to the folder containing your CSV files.
   
2. Ensure your CSV files have the following columns:

* Gene name

* log2FoldChange

* Gene description

3. Run the script.
