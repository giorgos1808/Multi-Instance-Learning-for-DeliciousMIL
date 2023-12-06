# Multi-Instance Learning with DeliciousMILDataset

## Description
This repository contains a notebook implementing Multi-Instance Learning (MIL) using the DeliciousMILDataset. The dataset consists of text documents with associated binary labels. 
The primary goal of this notebook is to explore and experiment with MIL approaches, comparing their effectiveness at both the document and sentence levels.

## Learning from Bags of Cases
The objective is to address the learning from bags of cases problem. The emphasis is on the most frequent of the 20 classes to transform it into 
a binary classification problem. Each document is considered as a bag of sentences. The following approaches are implemented:

1. **Grouping Sentences and Representing as Bags of Sentences**
   - Group the sentences of the training set.
   - Represent each sentence as a bag of sentences.
   - Document representation is based on the groups to which its sentences belong.

2. **Document Representation in Terms of Propositions**
   - Model each document in terms of all its propositions.
 
## Key Experiments

### Document-Level Experiment
In this experiment, the notebook works with vectorized text input at the document level. Multiple classifiers and hyperparameter settings are evaluated to assess their performance 
on the DeliciousMILDataset.

### Sentence-Level Experiment with Clusters-Based Input
The second experiment introduces a unique approach by leveraging k-means clustering to extract features from bags of words and sentences. This innovative method replaces the 
standard feature extraction method commonly found in scikit-learn. It offers more interpretability and customization in feature extraction while maintaining scalability for handling large datasets.

## Performance Metrics
The notebook reports the results of these experiments in terms of key performance metrics, including accuracy, precision, and recall. These metrics provide insights into the 
effectiveness of different MIL techniques and feature extraction methods on the DeliciousMILDataset.

## Usage
Explore the notebook to delve into the world of Multi-Instance Learning and gain insights into how innovative feature extraction methods can enhance the interpretability and 
scalability of your machine learning models.
