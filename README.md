# NLP_medication_management

# Background

ADHD affects a significant portion of US children, with primary care pediatricians often managing their treatment, including medication prescriptions. Existing studies on primary care adherence to ADHD management guidelines primarily rely on structured electronic health record (EHR) data, limiting detailed assessment of medication monitoring. Current national quality metrics like HEDIS measures focus on in-office follow-up but lack evidence-based treatment recommendations. Moreover, they overlook non-traditional communication routes, such as telehealth and telephone encounters, which play a significant role in medication management. 

# Project Summary:

This study aims to evaluate the accuracy of a large language model in identifying documentation of ADHD medication side effects in various clinical encounter notes, potentially enhancing quality measurement and patient outcomes.

# Dataset:

The dataset used consists of structured and unstructured (free text) EHR data (2015-2022) from 11 community primary care practices. It includes all office, telehealth, and telephone encounters related to ADHD for patients aged 6-11 years. To examine medication side effects documentation, the study focused on patients with more than two ADHD medication encounters, involving prescriptions of stimulants or non-stimulants by primary care physicians.

# Repository Structure:

The repo consists of the src folder, which has two files listed below:

1. text_preprocessing_training: This Python file contains the necessary code for processing text data from the notes, extracting feature embeddings from LLaMA-13b, and training the network using feature embeddings.

2. downstream_analysis:This notebook contains the codes used for downstream analysis and figures.


# Citations:

 1. 
