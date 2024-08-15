# Comparison of Few-shot and Traditional NER Models for Medical Text

## Overview

This project benchmarks the performance of few-shot learning (FSL) models against traditional named entity recognition (NER) models on medical text datasets. Utilizing five distinct medical datasets, the study compares the efficacy of three traditional NER models (BERT-Linear Classifier, BERT-CRF, SANER) with three FSL models (StructShot & NNShot, Few-Shot Slot Tagging, ProtoNER). The results highlight the challenges of applying FSL methods to medical texts, especially when working with small, noisy datasets, and emphasize the need for further research to improve FSL model performance in medical NLP.

## Key Objectives

**Benchmarking Few-shot Learning Models:** Evaluate the performance of state-of-the-art FSL models such as StructShot & NNShot, Few-Shot Slot Tagging (FS-ST), and ProtoNER on medical NER tasks.

**Comparison with Traditional NER Models:** Compare these FSL models with traditional NER models, including BERT-Linear Classifier, BERT-CRF, and SANER, to understand their relative strengths and weaknesses in low-resource settings.

**Analysis of Model Performance on Noisy and Clean Data:** Investigate how the quality of the dataset (e.g., level of noise and ambiguity) affects the performance of these models, particularly in few-shot scenarios.

## Datasets

The project utilizes five medical text datasets, each representing different aspects of the medical domain:

**1. MIMIC III:** A publicly available dataset containing de-identified health-related data associated with critical care patients.  
**2. N2C2 2018:** A dataset from the shared task focusing on adverse drug events (ADE) and medication extraction.  
**3. I2B2 2014:** A dataset used for the de-identification of longitudinal medical records.  
**4. BioNLP 2016:** Focused on extracting descriptions of genetic and molecular mechanisms from scientific articles.  
**5. SMM4H 2021:** A social media mining dataset for health applications, particularly for ADE mention extraction.  


