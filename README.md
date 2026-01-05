# Interpretable Prediction of Ligand-Protein Binding

This project introduces a **ligand-only framework** designed to predict ligand-protein binding affinities without the need for protein structural information.

By bypassing the requirement for high-resolution structures, this approach facilitates hit prioritization in settings where protein structures are unavailable, unreliable, or computationally expensive to model, such as **DNA-Encoded Library (DEL)** screens and **chemoproteomics**.

## 📂 Project Organization

The repository is structured as follows:

* **`embeddings/`**: Scripts for generating high-dimensional feature representations (fingerprints/descriptors) from various chemical databases.
* **`classifiers/`**: Implementations of **TabPFNv2** binary classifiers tailored for specific ligand-protein interaction datasets.
* **`results/`**: Final output files, performance metrics, and scripts for figure visualization and interpretability analysis.

---

## 📊 Data Availability

The database files required to run these models (including pre-processed data for BindingDB, DUD-E, DepMap, and BRD9 DEL) are hosted externally:

> [!IMPORTANT]
> **Download Data:** [Google Drive Link](https://drive.google.com/drive/folders/16vhVYHk1MJDK8n7P36uL1gruSRK_hNeo?usp=sharing)

| Dataset | Description |
| --- | --- |
| **BindingDB** | Large-scale experimental binding affinities. |
| **DUD-E** | Benchmarking dataset for molecular docking and screening. |
| **DepMap** | Cancer dependency data for target identification. |
| **BRD9 DEL** | Data from DNA-Encoded Library screens targeting BRD9. |

---

## 🛠️ Credits & Attribution

The core logic for embedding generation and classifier architecture is modified from the [ligand-discovery](https://github.com/ligand-discovery) repository.
