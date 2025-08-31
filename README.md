# EKG-Abnormal-Cardiac-Detection-using-ML

This repository utilizes an EKG dataset with normal and abnormal EKGs to detect abnormalities in cardiac physiology such as myocardial infarction, heart failure, bundle branch block, etc.  
The machine learning algorithm is a Convolutional Neural Network (CNN) built with TensorFlow for abnormal detection.  

The dataset is originally from [Kaggle – ECG Heartbeat Categorization Dataset](https://www.kaggle.com/datasets/shayanfazeli/heartbeat/data), which provides segmented and preprocessed ECG signals for heartbeat classification.  

## Dataset Modification  
For this repository, we created a **combined dataset** by merging the original **normal** and **abnormal** ECG files from Kaggle into a single file.  
- The combined dataset contains both classes (normal and abnormal) in one file.  
- For computational efficiency and demonstration purposes, the number of samples has been reduced to **300 data points** (150 normal + 150 abnormal).  
- Each sample has **188 ECG signal points** plus an additional column for the label (`0` = normal, `1` = abnormal).  

This preprocessing ensures easier loading, training, and reproducibility within the provided code.  
