# COMP0082 Coursework V2.02: Predicting the Subcellular Location of Proteins

## Overview

This project involves developing a machine learning model to predict the subcellular location of eukaryotic protein sequences. The goal is to classify proteins into five categories:

- **Cytosolic**: Inside the cell, but not in organelles.
- **Extracellular/Secreted**: Proteins secreted outside the cell.
- **Nuclear**: Proteins found in the nucleus.
- **Mitochondrial**: Proteins transported to mitochondria.
- **Other**: Proteins that don't fall into the above categories (e.g., prokaryotic proteins).

## Objective

Develop a model that classifies protein sequences into the above categories, with predictions including confidence levels (High, Medium, Low). The model should be able to run offline without external web services and should be evaluated using cross-validation.

## Data

The protein sequences are provided in **Fasta format** and categorized into:

- **Cytosolic** (2463 examples)
- **Extracellular/Secreted** (1236 examples)
- **Mitochondrial** (1023 examples)
- **Nuclear** (2736 examples)
- **Other** (2002 examples)

A **blinded challenge set** with 20 sequences will also be provided for final testing.

## Methodology

1. **Data Preprocessing**: Extract relevant features from protein sequences, such as sequence length, amino acid composition, isoelectric point, and sequence motifs.
  
2. **Model Selection**: Choose any appropriate machine learning technique (e.g., neural networks, SVMs, decision trees).
  
3. **Model Training**: Train the model using cross-validation on the provided dataset and evaluate performance using metrics like **Accuracy**, **F1 Score**, and **MCC**.
  
4. **Blinded Challenge**: Predict subcellular locations for the blinded challenge sequences, including confidence levels (High, Medium, Low).

5. **Report**: Submit a detailed report (2500 words max) discussing the problem, methodology, results, and analysis. Include a table of predictions for the blinded challenge.