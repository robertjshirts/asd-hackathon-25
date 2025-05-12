# ASD Prediction Project
## Overview
This repository contains our machine learning project for analyzing and predicting autism status using data from a questionnaire and some general demographic data.

This project includes:
- Requirements.txt - The python requirements needed to run the program
- ASD-Analysis.ipynb - The jupyter notebook including all of our work and data analysis
- 3 csv's for the input data:
  - test.csv - The main testing data
  - nonsynthetic.csv - The original dataset that the main testing data was generated from
  - test.csv - The test data, to be predicted to determine a final score

# Project summary
The goal of this project was to predict whether individuals are ASD based on demographics and answers to a questionnaire, and to train/evaluate a variety of machine learning models including:
- Logistic regression
- Random forest
- XGBoost
- CatBoost
- Neural networks

Each model was tuned using Optuna for hyperparameter optimzation and evaluated using a bunch of metrics due to our heavy imbalance with an only 20% minority of the target class. We also explored feature importance to understand which factors were most important for the models.

## Key observations:
At least according to our data set:
- 20% Of people are autistic
- Being white-european is heavily correlated with a high probility of an autism diagnosis
- People who didn't put down their ethnicity rarely have autism
- Being born with jaundice is somewhat correlated with an autism diagnosis
- Residing in the united states makes you more than 50% likely to have an autism diagnosis

# Project Setup and Running Instructions

## Setting up the Virtual Environment

1. Create the virtual environment:
   - On Windows:
   ```bash
   python3.12 -m venv .venv
   ```
   - On Unix/MacOS:
   ```bash
   python3.12 -m venv .venv
   ```

2. Activate the virtual environment:
   - On Windows:
     ```bash
     .venv\Scripts\activate
     ```
   - On Unix/MacOS:
     ```bash
     source .venv/bin/activate
     ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## Running Jupyter Notebook

1. Make sure your virtual environment is activated (you should see `(.venv)` in your terminal prompt)
   
   Note: You may be able to run without the virtual environment on windows, in which case you can skip steps 1 and 2 above.

3. Start Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

4. Your default web browser should open automatically with the Jupyter interface. If it doesn't, you can copy and paste the URL that appears in your terminal.

5. Navigate to and open the `ASD-Analysis.ipynb` notebook to start working.

## Deactivating the Virtual Environment

When you're done working, you can deactivate the virtual environment by running:
```bash
deactivate
``` 
## Hackathon Project

### The Team
Jake Malmrose - https://github.com/JakeMalmrose
Robbie Shirts - https://github.com/robertjshirtsc
Zachariah Hansen - https://github.com/ZachariahHansen

### The Task
https://github.com/Aabo-Home/hackathon-2025-asd-analysis

