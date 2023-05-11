# STAT 159 Group 20 Project: Housing Prices Prediction

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/UCB-stat-159-s23/project-Group20/HEAD)

## Introduction
This is a Final Project of Group 20 for STAT 159 Spring 2023. The project explores factors that impact the housing price, such as demographic, socioeconomic, and environmental factors. The data is obtained from a [Kaggle tutorial competition](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data) and can be found in the `data` folder. 

A JupyterBook of the main notebook `code_notebook.ipynb` can be found [here](https://ucb-stat-159-s23.github.io/project-Group20/).

## Project Description
The study starts with a introduction with a brief overview of the project's objectives and the data sources used in the analysis. Then, we did data importation and data cleaning. We created a 70/30 training/test dataset. For exploratory data analysis (EDA), we conducted descriptive statistics and visualizations, such as bar charts, histograms, and scatter plots. With the plots from EDA, we did feature selection to select the most relevant features for modeling using correlation analysis, feature importance techniques, and domain knowledge. 

We also conduct a simple ordinary least squares (OLS) regression to predict the outcome of interest using a subset of features. Then, we compared model performance using evaluation metrics such as R-squared, mean squared error, and mean absolute error. We provided the necessary packages and tests for this project, as well as the datasets and plots.

## Installation
Start by tying the following commands in your terminal:
- Create environment
  - Use `Makefile`: `make env`
  - Alternatively you can run the conda and python commands yourself
	  - To create a new conda environment based on the specifications defined in the `environment.yml` file: \
		`mamba env create -f environment.yml -p ~/envs/housing`
	  - To install a new IPython kernel into the Jupyter Notebook, specifically for the `housing` environment: \
		`python -m ipykernel install --user --name housingtools --display-name "IPython - housing"`
	  - Activate environment
		`conda activate housing`
- Install package
  - `pip install .`
- Build target specified in `Makefile`
  - `make all`

## Testing
- To run all tests on the functions: `pytest tools`


