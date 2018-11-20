# CS 7641 Assignment 1: Supervised Learning Classification

This project seeks to understand the computatitonal and predictive qualities of five classification algorithms (Neural Network, SVM, kNN, Decision Tree, and Boosted Trees). Each algorithm will be run for two binary classification datasets so that we can compare and contrast them for two different problems.

Dataset 1: Phishing Websites - available at https://www.openml.org/d/4534

Dataset 2: Gene Expression - available at https://www.kaggle.com/c/gene-expression-prediction

All the code is in following Jupyter Notebooks:
1. Phising_dataset.ipynb: Run all the cells sequentially to recreate my analysis on Phishing datset
2. Gene_expression.ipynb: Run all the cells sequentially to recreate my analysis on Gene Expression datset

Data Files:
Gene_Expression_Dataset: Preprocessed file, read below
Phising_dataset

# Requirements:
1. Jupyer Notebook
2. Python 3.5
3. Any web browser to run Jupyter notebook
4. Python Libraries needed:
	* scikitlearn
	* numpy
	* Pandas
	* seaborn
	* matplotlib

Note:

1. For running Jupyter notebooks dataset must be in the same folder as Jupyter Notebook

2. Some data processing for Gene_expression_Dataset data has been done in excel. Raw data from Kaggle had different dimension from the processed data given here.
For reshaping multiple rows for each GeneID has been converted into columns/features. 
Also, 15 derived variables like sum, mean and median on all 100 bins/features have been created.
Gene_Expression_Dataset file is the processed file after the above steps.

