# **Ma513 Project | Hands-On Machine Learning for Cybersecurity**
## Named Entity Recognition (NER) for Cybersecurity-Related Entities in Text

This repository contains the code and experiments for developing a NER model using various machine learning algorithms. The focus of this project is on exploring tree-based classifiers, from simple decision trees to more complex models like Random Forest and LightGBM (LGBM), and compare their performance to more complex, transfomer-based ones such as BERT. Through this approach, our aim was to build a robust NER model by applying the knowledge acquired in class to deepen our understanding of concepts like feature extraction, model selection, and performance evaluation.

**Table of Contents**<br>
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Model Development](#model-development)
- [Installation](#installation)

## Project Overview
This project began with the goal of exploring classical machine learning algorithms for NER, before progressing to more complex models like transformers. We started by using the Classification Learner plugin in MATLAB to explore various basic models, which provided us rapid insights into the model performance. These insights helped guide us towards tree-based models, culminating in the selection of the LightGBM classifier (LGBM) for its efficiency and performance on our NER task.

Key Steps:
Preprocessing Data: Preparing the dataset by tokenizing and extracting features from the text.
Feature Extraction: Developing custom features such as token length, presence of digits, and context-based features.
Model Exploration: Experimenting with a fine tree, Random Forest, and LightGBM classifiers.
Evaluation: Using performance metrics like accuracy, confusion matrix, and feature importance to select the best model.

## Model Development
Initial Exploration: We started with a fine decision tree model to establish a baseline and understand the context size needed for the task.
Random Forest: Next, we explored the Random Forest algorithm to increase the robustness and diversity of our model.
LightGBM (LGBM): Finally, we settled on LightGBM, a gradient boosting model, for its superior handling of high-dimensional data, efficiency, and robustness.
For more details, please refer to the Model Selection section.

## Dataset
The dataset used for this project consists of annotated NER data in the format of JSON Lines files. It contains tokens and their corresponding NER tags. You can load and preprocess these datasets using the provided functions in the code.

File Format:
Training Data: NER_TRAINING.jsonl
Validation Data: NER_VALIDATION.jsonl
Testing Data: NER_TESTING.jsonl
The features are extracted from the tokens in these files, and the NER tags are used to train the model.

## Installation
To run the code and experiments, ensure you have the following dependencies installed:

Python 3.x
pandas
scikit-learn
lightgbm
matplotlib (optional, for plotting)
Jupyter Notebook (optional, for interactive exploration)
