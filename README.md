# Machine_Learning_Project
This repository contains the documentation of our work in the course project of BITS 464 Machine Learning. The course introduced us to several fundamental concepts of Machine Learning such as Regression, classification, Neural Networks, SVMs. As part of our final project, we made this repository.

Inspired by the paper "DNA Sequence Classification by Convolutional Neural Network" by Nguyen et al., we carried out our research.
We first attempted by the implementation of the paper.
Due to the computational resources present, out of the 12 datasets mentioned in the paper, we selected the H3K4me1 to work with. A broad overview of our approach is below
- We performed an exploratory analysis to understand the dataset. We removed any noise present here.
- Every sequence used a 3-mer representation and one-hot encoding embedding method which was then implemented.
- We replicated the model architecture present and chose the best hyperparameters.
- The dataset used and the code for base model implementation can be found here.

## Further changes made include:

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
