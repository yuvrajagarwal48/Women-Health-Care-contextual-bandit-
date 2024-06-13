# Contextual Bandit Project
=====================

## Description
This project implements a contextual bandit algorithm using logistic regression as the base algorithm. The goal is to optimize the cumulative reward in a multi-label classification problem.

## About Dataset
(https://www.kaggle.com/datasets/ravikrishnareddy/women-health-care-requirements/data)

## Features
* Implements a contextual bandit algorithm using logistic regression as the base algorithm
* Optimizes the cumulative reward in a multi-label classification problem
* Uses the `contextualbandits` library for online learning


## How to Use
1. Load the train and test data using `load_data.py`.
2. Preprocess the data using `preprocess_data.py`.
3. Train the contextual bandit model using `train_model.py`.
4. Evaluate the model using `evaluate_model.py`.
5. Use the model to predict actions for the test data using `predict_actions.py`.

## Model Saving
The model can be saved using the `cloudpickle` library. To save the model, use the following code:
```python
import cloudpickle
cloudpickle.dump(models[3], open("sft_model.pkl", "wb"))
