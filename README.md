# ECG wave analysis using neurokit2

## Description

- The dataset used is available at: https://www.kaggle.com/datasets/bjoernjostein/china-12lead-ecg-challenge-database .
It consists of 3453 .mat and 3453 .hea files.
Each .mat files consists of a numpy array of size (12,samples) where 12 signify the number of leads in order: lead I, lead II, lead III, aVR, aVL, aVF, V1, V2, V3, V4, V5, and V6. The number of samples vary from file to file.
Each .hea file consists of data about the patient and calibarations related to ECG readings.
