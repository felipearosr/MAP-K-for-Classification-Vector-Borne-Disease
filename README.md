# Vector Borne Disease Diagnosis Prediction

This Jupyter notebook presents a machine learning model aimed at predicting possible diagnoses of vector-borne diseases based on clinical symptoms. The notebook employs a logistic regression model to predict the probabilities of various diseases and ranks them using the Mean Average Precision at K (MAP@K) metric. This approach is particularly useful in medical diagnostics, where identifying a shortlist of potential diseases can significantly streamline further testing processes.

## Overview

The primary goal of this notebook is to demonstrate the application of MAP@K for evaluating a multi-class classification model in the context of vector-borne disease diagnosis. By predicting the top three most probable diagnoses and evaluating these predictions using MAP@K, we can assess the model's ability to correctly identify relevant diseases within the top-ranked predictions.

## Dataset Description

The dataset used in this notebook includes symptoms and diagnoses of various vector-borne diseases. Each row represents a unique patient case, with features indicating the presence or absence of specific symptoms. The 'prognosis' column contains the actual disease diagnoses.

## Model Description

We utilize a Logistic Regression model to handle the multi-class classification problem. The model is trained to predict the probability of each possible diagnosis given the symptoms. These probabilities are then used to determine the top three most likely diseases for each case.

## Evaluation Metric

The performance of the model is evaluated using the MAP@K metric, with K set to 3. This metric considers both the precision of the top K predictions and their order, making it a stringent and informative measure for ranking problems.
