# Exploring Cellular Automata and Deep Learning Techniques for Refining Low-Confidence Regions in AlphaFold-Generated Models

### [🌐 Versión en español / Spanish version](README.md)

## Description

AlphaFold2 predicts protein structures with atomic-level accuracy, but it generates a single static conformation per protein. This is insufficient to represent the heterogeneous, dynamic nature of intrinsically disordered regions (IDRs) and highly flexible regions such as long loops, whose accuracy decreases systematically as their length increases.

This project explores the design of a hybrid model that integrates Cellular Automata (CA) and Deep Learning (DL) techniques to generate conformational ensembles in low-confidence structural regions (pLDDT < 70), aiming to balance structural rigor with computational efficiency compared to traditional Molecular Dynamics-based methods.

## Objectives

### General

To design a model based on CA and DL techniques for refining low structural confidence regions (low pLDDT) in AlphaFold-generated protein models.

### Specific

1. Analyze AlphaFold's current limitations in predicting intrinsically disordered regions or regions with low structural confidence, through a systematic review.
2. Design a conceptual model integrating CA and DL for refining such regions.
3. Develop an experimental tool implementing the model, trained on AlphaFold–native structure pairs.
4. Evaluate the approach's effectiveness using structural and confidence metrics, comparing against original AlphaFold models.

## Technologies

* ***Language***: Python ≥ 3.14
* ***DL***: PyTorch ≥ 2.10
* ***Bioinformatics***: BioPython ≥ 1.86, PDB format
* ***Data analysis***: NumPy ≥ 2.4, Pandas ≥ 3.0, SciPy
* ***Structural evaluation***: TM-align / TM-score, pLDDT
* ***Visualization***: Seaborn, PyMOL
* ***Environments***: Jupyter Notebook, Google Colab (GPU)