# ASSIGNMENT 3: UNSUPERVISED LEARNING

The objective is to apply unsupervised learning algorithms like clustering and dimensionality reduction. In the first part, we run various clustering algorithms on the datasets and note the observations. In the second part, dimensionality reduction (PCA) has been used to reduce to feature space for both the datasets and how this affects clustering is studied. Then in final part, we study how the clustering algorithms and the dimensionality reduction (PCA) affect the accuracy of a dataset by passing the transformed data through a Neural Network.


All the code is in following Jupyter Notebooks:
1. ASSIGNMENT 3.ipynb: Run all the cells sequentially to recreate my analysis for Assignment 3

### Data Files:
1. Gene_Expression_Dataset: Preprocessed file, read below
2. Phising_dataset

### Requirements:
1. Jupyer Notebook
2. Python 3.5
3. Any web browser to run Jupyter notebook
4. Python Libraries needed:
	* scikitlearn
	* numpy
	* Pandas
	* seaborn
	* matplotlib

### Note:

1.For running Jupyter notebooks dataset must be in the same folder as Jupyter Notebook

2. Some data processing for Gene_expression_Dataset data has been done in excel. Raw data from Kaggle had different dimension from the processed data given here.
For reshaping multiple rows for each GeneID has been converted into columns/features. 
Also, 15 derived variables like sum, mean and median on all 100 bins/features have been created.
Gene_Expression_Dataset file is the processed file after the above steps.
