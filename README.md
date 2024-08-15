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

## Methodology

**Model Selection:** We selected six NER models—three traditional models (BERT-Linear Classifier, BERT-CRF, SANER) and three few-shot learning models (StructShot & NNShot, Few-Shot Slot Tagging, ProtoNER).

**Training and Evaluation:** Models were trained and evaluated using various data availability scenarios, including 1-shot, 5-shot, 10% of the data, and the full dataset. This allowed us to simulate real-world conditions where only limited annotated data is available.

**Performance Metrics:** We used F1-scores as the primary metric to evaluate model performance across different datasets and settings.

## Usage

To reproduce the experiments:

Clone the repository and ensure you have the necessary datasets available.  
Install dependencies using the provided requirements.txt.  
Run the notebooks to preprocess the data, train the models, and evaluate their performance on the selected datasets.  

## Requirements

· Python 3.x  
· Hugging Face’s Transformers library  
· PyTorch  
· scikit-learn  
· NumPy, Pandas, and Matplotlib for data handling and visualization  

## Contributions

1. Comprehensive Benchmarking: This project is one of the first to benchmark few-shot NER models against traditional models using medical text datasets, providing valuable insights into their strengths and limitations.

2. Dataset Reconstruction for Few-shot Learning: The datasets were reconstructed to fit few-shot learning scenarios, which involved creating K-shot-N-way configurations to simulate low-resource environments.

3. Guidelines for Future Research: The findings highlight the need for developing more robust FSL models and standardized datasets that accurately reflect real-world challenges in medical NLP.

## Acknowledgments

This research was supported by the National Institute on Drug Abuse (NIDA) of the National Institutes of Health (NIH).
