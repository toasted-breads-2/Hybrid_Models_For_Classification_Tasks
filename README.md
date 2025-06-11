# Introduction
This repository contains the documentation of our work in the course project of BITS 464 Machine Learning. The course introduced us to several fundamental concepts of Machine Learning such as Regression, classification, Neural Networks, SVMs. As part of our final project, we made this repository. 

***Please explore the Presentation attached in the repo that documents our entire progress.***

This project aims to classify whether histones bind (wrap) around given DNA sequences using deep learning-based approaches. Histones are positively charged proteins that play a central role in DNA compaction by organizing and packaging DNA into structural units known as nucleosomes. The interactions between histones and DNA are fundamental to processes like gene regulation, chromatin remodeling, and epigenetic modifications.

Understanding these interactions can provide deep biological insights and aid in decoding complex regulatory mechanisms underlying various diseases, including cancer.

## Inspiration
This work is inspired by the paper "DNA Sequence Classification by Convolutional Neural Network" by Nguyen et al.. The study explores how deep learning, particularly Convolutional Neural Networks (CNNs), can be utilized to extract patterns and learn sequence-specific features that distinguish binding from non-binding sites.

## Problem Statement
Given a set of DNA sequences, the objective is to predict whether a histone will bind to that region or not. This is essentially a binary classification problem where the input is a nucleotide sequence and the output is a label indicating histone interaction.

## Dataset
The dataset consists of labeled DNA sequences extracted from biological databases and processed to balance class distributions. Sequences are preprocessed and standardized for uniform input length.

## Approach for Implementation
Due to the computational resources present, out of the 12 datasets mentioned in the paper, we selected the H3K4me1 to work with. A broad overview of our approach is below
- We performed an exploratory analysis to understand the dataset. We removed any noise present here.
- Every sequence used a 3-mer representation and one-hot encoding embedding method which was then implemented.
- We replicated the model architecture present and chose the best hyperparameters.
- The dataset used and the code for base model implementation can be found here.

## Further changes made include
To think of a novel approach, we brainstromed and came up with the following:
Broadly, the paper could be divided into three segments:
- Sequence Representation
- Sequence Embedding
- Model Architecture

We started experimenting with every segment. All the successful experiments have been documented. These are:

1. Hyperparameter Tuning
2. Utilisation of 4 mer representation
3. Utilisation of Word2Vec embedding
4. Utilisation of Hybrid models

Code used for every model has been attached in the repository.

## Tools & Frameworks
- Python
- TensorFlow / Keras
- NumPy, Pandas
- Matplotlib, Seaborn for visualization

## Evaluation
Models were evaluated using standard classification metrics:
- Accuracy
- Precision, Recall, F1-score
- ROC-AUC Curve

## Repository Structure
HK4me1.txt: Contains the raw dataset used.
dataset.txt: Is the cleaned dataset after preprocessing.
OnehotEncoding_CNN.ipynb: Jupyter notebook for base model implementation.
OnehotEncoding_CNN_hyperparam_optim.ipynb: Jupyter notebook for hyperparameter tuning of base model cnn.
onehot_cnn+bilstm.ipynb: Jupyter notebook for hybrid model.
word2vec_cnn+bilstm.ipynb: Jupyter notebook for Word2Vec embedding and hybrid model implementation.
4mer_Word2Vec_CNN+LSTM.ipynb: Jupyter notebook for 4mer representation and hybrid model.
README.md: Project overview and instructions.
ML Project Report (1).pdf : Project report.
ML Project Presentation.pdf: Presentation.
