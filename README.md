# NLP_medication_management

# Background

ADHD affects a significant portion of US children, with primary care pediatricians often managing their treatment, including medication prescriptions. Existing studies on primary care adherence to ADHD management guidelines primarily rely on structured electronic health record (EHR) data, limiting detailed assessment of medication monitoring. Current national quality metrics like HEDIS measures focus on in-office follow-up but lack evidence-based treatment recommendations. Moreover, they overlook non-traditional communication routes, such as telehealth and telephone encounters, which play a significant role in medication management. 

# Project Summary:

This study aims to evaluate the accuracy of a large language model in identifying documentation of ADHD medication side effects in various clinical encounter notes, potentially enhancing quality measurement and patient outcomes.

# Dataset:

The dataset used consists of structured and unstructured (free text) EHR data (2015-2022) from 11 community primary care practices. It includes all office, telehealth, and telephone encounters related to ADHD for patients aged 6-11 years. To examine medication side effects documentation, the study focused on patients with more than two ADHD medication encounters, involving prescriptions of stimulants or non-stimulants by primary care physicians.

# Repository Structure:

The repo consists of the src folder, which has two files listed below:

1. : data_processing and modellingThis folder contains python files required for processing text data from the notes before applying the transformer model.

2. downstream analysis:This folder contains notebooks used to obtain results for the research.
  
    a. The Training_ClinicalBERT notebook trains the network using dataset mentioned, and the trained weights are saved for further use.
  
    b. The Deployment_Val_Test_Set notebook uses the saved weights to obtain the results for validation and test set (annotated notes).
  
    c. The Final_Deployment_notebook uses the saved weights and predicts the labels and "BT_y/n" for unannotated notes, and the predictions are saved for further analysis.           (BT: Behavioral Therapy)



# Citations:

 1. https://simpletransformers.ai/docs/binary-classification/
 2. Zima BT, Mangione-Smith R. Gaps in quality measures for child mental health care: an opportunity for a collaborative agenda. Journal of the American Academy of Child and Adolescent Psychiatry. 2011;50(8):735-737.
 3. National Committee for Quality Assurance. Follow-up care for children prescribed ADHD medication. Available at: http://www.ncqa.org. . Accessed October 24, 2019.
 4. Zima BT, Murphy JM, Scholle SH, et al. National quality measures for child mental health care: background, progress, and next steps. Pediatrics. 2013;131 Suppl 1:S38-49.
 5. Casalino LP, Gans D, Weber R, et al. US Physician Practices Spend More Than $15.4 Billion Annually To Report Quality Measures. Health Aff (Millwood). 2016;35(3):401-406.
 6. Schuster MA, Onorato SE, Meltzer DO. Measuring the Cost of Quality Measurement: A Missing Link in Quality Strategy. Jama. 2017;318(13):1219-1220.
