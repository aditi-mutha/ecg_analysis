# ECG wave analysis 
A simple EDA of raw ECG readings.

## Dataset

- The dataset used is available at: https://www.kaggle.com/datasets/bjoernjostein/china-12lead-ecg-challenge-database .
- It consists of 3453 .mat and 3453 .hea files.
- Each .mat files consists of a numpy array of size (12,samples) where 12 represents the number of leads in order: lead I, lead II, lead III, aVR, aVL, aVF, V1, V2, V3, V4, V5, and V6. The number of samples vary from file to file.
- Each .hea file contains data about the patient and calibarations related to ECG readings.

## Q1.ipynb
- Calculation of ST segment elevation using S peaks and T onsets.
- ST segment elevation may lead to Myocardial Infarction (MI) if the readings are:
  - atleast 1mm for male.
  - atleast 0.5 mm for female.

## Q2.ipynb
- P wave morphology analysis for lead I, lead II and V1.
- Analysis is based on: P wave duration, monophasic/biphasic P wave, amplitude of P wave, and PR interval.

## Q3.ipynb
- An algorithm using 1D CNN for lead type detection based on wave morphology.
- Used various features like: P peaks, P onsets, P offsets, Q peaks, R onsets, R offsets, S peaks, T peaks, T onsets and T offsets.

## Q4.ipynb
- A simple visualization of P peaks, Q peaks, S peaks, T peaks, P onsets and T offsets for all the 12 lead types.
