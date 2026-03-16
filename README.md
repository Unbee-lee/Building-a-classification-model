## Overview
The task is to build a classification model that can accurately predict the vegetation condition of each land
parcel on Wadjuk Noongar country into the three categories, which are ‘Healthy’, ‘Degraded’ and ‘AtRisk’.

Understanding the condition of vegetation is essential for maintaining biodiversity, managing fire risk, guiding cultural burns, and protecting culturally significant areas.
The given dataset is ‘Assignment2025S2.sqlite’, where each record contains various indicators of environmental condition, such as vegetation health, soil properties, moisture availability, proximity to water, and signs of human or invasive
species disturbance. 

There are a total of 5500 samples across two tables, which are ‘train’ and ‘test’. Before data classification, data preparation was conducted, including the identification and removal of
irrelevant attributes, the detection and handling of missing entries, the detection and handling of duplicates,
the selection of suitable data types for attributes and data transformation. 

For data classification, 4 models were used, which are K-NN, Decision tree, Naive Bayes and SVM. The Models were evaluated by using a
confusion matrix, accuracy, precision, recall and F1-score. The Naive Bayes model and the SVM model were considered best for the task, achieving 80% estimated accuracy and 88% estimated accuracy, respectively.

## Project Report
For a detailed analysis and methodology, please refer to the full report:

https://github.com/Unbee-lee/Building-a-classification-model/blob/main/Report/Report.pdf






