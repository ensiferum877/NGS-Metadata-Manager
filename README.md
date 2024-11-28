# Project Introduction

This repository demonstrates an automated approach to identifying, acquiring, and analyzing specific types of publicly available genomic data to support biomarker discovery for Parkinson's Disease (PD). The project focuses on single-cell transcriptomic data generated from biological fluids, particularly whole blood or peripheral blood mononuclear cells (PBMCs).

KEYWORDS: Data mining - Bioinformatics - Gene Expression Omnibus - Large Language Models - AI-assisted curation - scRNA sequencing - Biomarker discovery

Why Biological Fluids and Single-Cell Transcriptomics?
Clinical Utility: We are interested in identifying biomarkers that can be easily and non-invasively obtained for the clinical detection of PD. Biological fluids, especially blood, offer a promising avenue for developing such diagnostic tools.

Enhancing Resolution: Previous analyses of bulk sequencing data have revealed transcriptomic differences between PD patients and healthy controls. However, these differences are often subtle at the bulk level. We hypothesize that by profiling these samples at single-cell resolution, we can maximize our ability to detect and characterize these differences, potentially uncovering cell type-specific biomarkers that are masked in bulk analyses.

Project Components
This project encompasses three main areas:

Programmatic Extraction of Data: Utilizing Python libraries to interact with the Gene Expression Omnibus (GEO) database, perform automated querying based on specific search criteria, and efficiently download relevant dataset metadata.

AI-Driven Analysis of Experimental Metadata: Employing Llama 3.2 via Ollama for AI-driven data labeling of GEO experimental metadata, enhancing our ability to identify relevant datasets accurately.

Single-cell Transcriptomics Analysis: Conducting end-to-end scRNA-seq analysis of 10X Genomics data using Python libraries such as Scanpy and scv-tools, to uncover cell type-specific signatures and potential biomarkers.

Data Availability
This project involves two main types of data:

Gene Expression Omnibus (GEO) Data:

Experimental Metadata: We query GEO for studies related to Parkinson's disease, focusing on single-cell RNA sequencing data from blood or PBMC samples. This metadata includes information about study design, sample characteristics, and experimental protocols.
scRNA-seq Data: For selected studies, we download the actual single-cell RNA sequencing data. This typically includes gene expression matrices, cell annotations, and related files necessary for downstream analysis.
AI-Generated and Processed Data:

Llama 3.2 7B via Ollama Output: We use the Llama 3.2 7B model, accessed through Ollama, to analyze and classify the experimental metadata from GEO. This AI-generated data includes classifications of studies based on technology used, sample type, and relevance to our research question, as well as justifications for these classifications.
Curated Dataset: The final output of our data collection and AI analysis process is a curated dataset that combines information from GEO metadata, AI classifications, and links to the relevant scRNA-seq data files.
🧫 Conclusion
To be continued

NOTE
Note on Ollama Installation
This notebook **DOES NOT cover the installation of Ollama or the Docker generation for this project. For detailed instructions on installing Ollama and structuring its output, please refer to:

Llama 3.2 Tutorial: How to Use Llama 3.2 (7B, 13B, 70B) Locally

It's recommended to set up Ollama before running the notebook to ensure all AI-assisted data curation steps function correctly.
