# Personalized-Medicine-Redefining-Cancer-Treatment
## 1. Business Problem
## 1.1. Description
Source: https://www.kaggle.com/c/msk-redefining-cancer-treatment/

Data: Memorial Sloan Kettering Cancer Center (MSKCC)

Download training_variants.zip and training_text.zip from Kaggle.

## Context:
Source: https://www.kaggle.com/c/msk-redefining-cancer-treatment/discussion/35336#198462

## Problem statement : 
Classify the given genetic variations/mutations based on evidence from text-based clinical literature.

## 1.2. Source/Useful Links
Some articles and reference blogs about the problem statement

- https://www.forbes.com/sites/matthewherper/2017/06/03/a-new-cancer-drug-helped-almost-everyone-who-took-it-almost-heres-what-it-teaches-us/#2a44ee2f6b25
- https://www.youtube.com/watch?v=UwbuW7oK8rk
- https://www.youtube.com/watch?v=qxXRKVompI8
## 1.3. Real-world/Business objectives and constraints.
- No low-latency requirement.
-Interpretability is important.
- Errors can be very costly.
- Probability of a data-point belonging to each class is needed.
## 2. Machine Learning Problem Formulation
## 2.1. Data
## 2.1.1. Data Overview
Source: https://www.kaggle.com/c/msk-redefining-cancer-treatment/data
We have two data files: one conatins the information about the genetic mutations and the other contains the clinical evidence (text) that human experts/pathologists use to classify the genetic mutations.
Both these data files are have a common column called ID
### Data file's information:

- training_variants (ID , Gene, Variations, Class)
- training_text (ID, Text)

## 2.2. Mapping the real-world problem to an ML problem
## 2.2.1. Type of Machine Learning Problem
There are nine different classes a genetic mutation can be classified into => Multi class classification problem

## 2.2.2. Performance Metric
Source: https://www.kaggle.com/c/msk-redefining-cancer-treatment#evaluation

### Metric(s):

- Multi class log-loss
- Confusion matrix
## 2.2.3. Machine Learing Objectives and Constraints
### Objective: Predict the probability of each data-point belonging to each of the nine classes.

### Constraints:

- Interpretability
- Class probabilities are needed.
- Penalize the errors in class probabilites => Metric is Log-loss.
- No Latency constraints.
