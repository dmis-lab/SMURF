# SMURF
Python implementation of SMURF (SMURF: Machine learning pipeline for discovering cancer type specific driver mutations and diagnostic markers).

## Abstract
To identify driver mutations and accurately distinguish them from passenger mutations, it is important to analyze somatic mutation data at the variant level. Also, for the recently emerging technology of liquid biopsies which use the somatic mutation signatures of the DNA fragments in blood, it is necessary to obtain an optimal mutation set (i.e., diagnostic markers) that can be used to accurately classify multiple cancer types. 
 In this work, we present SMURF, a machine learning pipeline for analyzing somatic mutation profiles across 31 cancer types at the variant level. SMURF consists of two main components: SMURF-OVR and SMURF-Multi. SMURF-OVR uses one-vs-rest binary random forest classifiers for the cancer types, and identifies cancer type specific driver mutations based on the feature importance scores obtained by the one-vs-rest
random forest classifiers. Driver mutations predicted in SMURF-OVR have high pathogenicity and the predicted cancer type specific mutation sets are enriched with true cancer type specific driver mutations in the following six cancer types: colorectal adenocarcinoma (COADREAD), non small cell lung cancer (NSCLC), acute myeloid leukemia (LAML), skin cutaneous melanoma (SKCM), thyroid carcinoma (THCA), and breast invasive carcinoma (BRCA). SMURF-Multi identifies the optimal mutation diagnostic marker set that accurately classifies multiple cancer types using the feature importance scores obtained by a multi-class random forest classifier. Compared with the other known panels of mutations, we show that our set of mutations with the highest feature important scores is more useful for classifying multiple cancer types. Using the feature importance scores of the random forest classifiers, we were able to identify cancer type specific driver mutations and diagnostic markers. We hope that SMURF will be utilized in cancer diagnostic applications such as liquid biopsies.

## Pipeline
![SMURF](SMURF.png)

## Requirements
- python (recommend installing Anaconda2)
- numpy
- scipy
- sklearn
- pandas
- time

## Contacts
For help or issues using SMURF, please contact Sungjoonpark (sungjoonpark (at) korea.ac.kr).
