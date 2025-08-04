# SDUEBA: Subgroup Detection Using Embedding-Based Approaches

---

This repository contains the showcase of **SDUEBA**, a scalable and interpretable pipeline for Subgroup Discovery (SD) using modern embedding techniques, clustering algorithms, and rule induction methods. This work was developed as part of the Bachelor's thesis *"Subgroup Detection Using Embedding-Based Approaches"* by Matyáš Veselý at the Faculty of Nuclear Sciences and Physical Engineering, Czech Technical University in Prague (FNSP CTU), in collaboration with Workday Prague.

**Thesis PDF:** to be published

**Author:** Matyáš Veselý  
**Institution:** Faculty of Nuclear Sciences and Physical Engineering, Czech Technical University in Prague (FNSP CTU)  
**Supervisor:** Ing. Jiří Franc, PhD.  
**Consultant:** Ing. Viktor Brada (Workday Prague)

> **Note:** This repository is intended as a showcase of the SDUEBA pipeline developed during the thesis. It is not designed to function as a fully general-purpose Python library.

If you have any questions, comments, or issues running the code, please do not hesitate to contact the author at **veselm73@cvut.cz**.

---

## Overview

Subgroup Discovery aims to identify subpopulations in data that differ significantly with respect to a target variable. Traditional SD methods often suffer from poor scalability and limited flexibility.

**SDUEBA** introduces a new approach based on the following components:

- Embedding generation (Word2Vec, BERT)
- Clustering of instance embeddings (e.g.,Agglomerative, k-means, HDBSCAN, TSPG clustering)
- Rule induction using decision trees
- Interpretable subgroup scoring and filtering

The pipeline is modular and capable of handling large, high-dimensional, and heterogeneous datasets.

---

## Datasets

The following datasets are used in this repository to demonstrate the method:

1. **Mushroom** – interpretable categorical dataset with clear subgroups.  
   *Source:* Schlimmer, J. C. (1987). Mushroom dataset. Originally from G. H. Lincoff, *The Audubon Society Field Guide to North American Mushrooms* (1981). UCI Machine Learning Repository. [https://archive.ics.uci.edu/dataset/73/mushroom](https://archive.ics.uci.edu/dataset/73/mushroom)

2. **Diabetes** – real-world clinical dataset with binary target.  
   *Source:* Strack, B., DeShazo, J. P., Gennings, C., Olmo, J. L., Ventura, S., Cios, K. J., & Clore, J. N. (2014). *Impact of HbA1c measurement on hospital readmission rates: Analysis of 70,000 clinical database patient records*. BioMed Research International, 2014  
   [https://archive.ics.uci.edu/dataset/296/diabetes](https://archive.ics.uci.edu/dataset/296/diabetes)

3. **US Traffic Accidents** – large, multiclass dataset.  
   *Source:* Moosavi, S., Samavatian, M. H., Parthasarathy, S., & Ramnath, R. (2019). *A countrywide traffic accident dataset.*  
   [https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents](https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents)

Each dataset is preprocessed and presented through Jupyter notebooks with all intermediate outputs and visualizations included.

---

## Running the Notebooks

The `gensim` library used for Word2Vec training may not be compatible with the latest versions of `NumPy`. To avoid runtime errors, it is advisable to restart your Python environment (e.g., Jupyter kernel or Colab runtime) after installing all dependencies before running the code.

