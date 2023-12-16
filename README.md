# w281-project


This directory contains the set of files used to explore and create a model for the Intel Image Dataset.

# Imporant Files :

- project_proposal.ipnyb - Contains the initial EDA for the project
- feature_engineering.ipynb - First part of the model pipeline.  Loads the images and creates feature vectors in a pandas Dataframe, finally storing it in a parquet file.
- tSNE.ipynb - Notebook used to visualize the tSNE plots
- logistic_regression.ipynb - Classifier using logistic regression.
- svm.ipynb - Classifier using Support Vector Machines

The remaining files are scratch files of some sort or another.

## Running

You will need a Kaggle API key loaded into your home directory in the .kaggle directory.  See https://github.com/Kaggle/kaggle-api?tab=readme-ov-file#api-credentials for the latest instructions on how to set that up.

Run the feature_engineering.ipynb notebook first, it will generate a series of parquet files containing the feature vectors.

Run eitiher the logistic_regression.ipynb or svm.ipynb notebooks to run the models and evaluate their accuracy.  These notebooks consume the parquet files from the previous step.
