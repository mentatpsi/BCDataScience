# Boston University Metropolitan CS 677 Data Science Final Project
As part of an intensive 7 week course on Data Science fundamentals, I selected as my final project an implementation of Machine Learning and Data Science on a Breast Cancer study from Memorial Sloan Kettering Cancer Center from 2018. All data was made available on cBioPortal and I've added it here as well. 

## Instructions
Open the Jupyter Notebook (.ipynb) in the code section. The whole Notebook should be loadable in browser. This can also be downloaded locally but requires installing Python and Jupyter (can be installed through pip install).

## Limitations
The prediction engines used I believe assume numerical data types. The loss functions for instance in a Neural Network with a logistic regression activation work using partial dervivatives that are a concept in Continous Mathematics (Calculus) that might need a change for a nominal data attribute. For the scope of the project, I have used algorithms that should work on nominal feature sets, and might just need tweaks through Pipelines, or work by more experienced Data Scientists and Medical Researchers. Over time this will be made to focus on nominal data sets to help with prediction validity. 

## Features
In this study we perform relational data analysis, we perform several machine learning algorithms. We end it with creating a contingency table to find association between gene mutations to possibly help visualize relations across gene networks that were discovered in the decision tree step. The Genes choosen to build the contigency table is non-deterministic, running this locally will produce a different set each time. 

## Purpose
The purpose of this analysis was to help researchers with a collection of tools for data science. It contains query functions, dataframes based on clinical outcome, relational data mapping, and more. I have provided some analysis of the genetics based on small research into each gene mutation. My background is Computer Science, with some minor Computational Biology work. I have highlighted as well some genes that have only been present in each outcome.

I hope this serves a greater purpose to help out researchers.


### Algorithms

#### Random Tree Ensemble
A Random Tree Ensemble is a collection of Decision trees with non-deterministic properties designed to prevent over-fitting through random selection of sample training data and feature sets (columns - in our case gene mutations). They construct a decision tree through usuage of information entropy to enhance the gain of information across a decision node. These trees then form a collection of decision makers that vote on a classification together.

#### Neural Network
The neural network used focuses on a logistic regression activation function, which works through passing a linear regression through a sigmoid function to inspire logical classifcation (binary). We attempt to predict survival based on gene mutations.  

#### Naive Bayes
Naive Bayes employs conditional probabilities and Bayes Theorem to determine class. It is called Naive because it employs the notion of independence to determine class which allows for unique mathematical operations not possible in dependence.


