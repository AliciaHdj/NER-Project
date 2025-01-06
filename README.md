# **Ma513 Project | Hands-On Machine Learning for Cybersecurity**
## Named Entity Recognition (NER) for Cybersecurity-Related Entities in Text

This repository contains the code and experiments for developing a NER model using various machine learning algorithms. The focus of this project is on exploring tree-based classifiers, from simple decision trees to more complex models like Random Forest and LightGBM (LGBM), and compare their performance to more complex, transfomer-based ones such as BERT. Through this approach, our aim was to build a robust NER model by applying the knowledge acquired in class to deepen our understanding of concepts like feature extraction, model selection, and performance evaluation. <br>
Our whole approach is deailed in the corresponding written report (Ma513_16__AliciaHEDDADJ_AliyahPARFAIT.pdf), and our final results can be found in Predictions.zip and Models.zip files.

**Table of Contents**<br>
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Model Development](#model-development)
- [Installation](#installation)

## Project Overview
This project began with the goal of exploring classical machine learning algorithms for NER, before progressing to more complex models like transformers. We started by using the Classification Learner plugin in MATLAB to explore various basic models, which provided us rapid insights into the model performance. These insights helped guide us towards tree-based models, ending in the selection of the LightGBM classifier (LGBM) for its efficiency and performance on our NER task. In parallel, we also tried exploring transformer-based models despite our constraints in resources.

**Key Steps** <br>
Preprocessing Data : Preparing the dataset by tokenizing and extracting features from the text. <br>
Feature Extraction : Developing custom features such as token length, presence of digits, and context-based features. <br>
Model Exploration : Experimenting with various tree classifiers and more complex models. <br>
Evaluation : Using performance metrics like accuracy, confusion matrix, and feature importance to select the best model. <br>

## Model Development
Initial Exploration : We started with a fine decision tree model to establish a baseline and understand the context size needed for the task. <br>
Random Forest: Next, we explored the Random Forest algorithm to increase the robustness and diversity of our model. <br>
LightGBM (LGBM) : Finally, we settled on LightGBM, a gradient boosting model, for its superior handling of high-dimensional data, efficiency, and robustness. <br>
BERT : Simultaneously, we tried developping a basic "bert-base-cased" model to explore and compare its performance to classical machine learning algortihms. <br>

## Dataset
The dataset used for this project consists of annotated NER data in the format of JSON Lines files. It contains samples composed of unique ids, tokens and their corresponding NER tags. The files are exctracted directly from the subject's github repository, so loading and preprocessing these datasets can be done using the provided functions in the code.

**File Format** <br>
Training Data : NER_TRAINING.jsonl <br>
Validation Data : NER_VALIDATION.jsonl <br>
Testing Data : NER_TESTING.jsonl <br>
The features are extracted from the tokens in these files, and the NER tags are used to train the model.

## Installation
The notebook containing the code was made with the following versions :
- Python 3.10.12
- Pandas 2.2.2
- Scikit-learn 1.6.0
- Lightgbm 4.5.0
- Matplotlib 3.8.0
