This project seeks to understand the behavioral and computatitonal and predictive qualities of four random search optimzation methods:

Randomized Hill Climb (RHC)
Simulated Annealing (SA)
Genetic Algorithms (GA)
Mutual Information Maximizing Input Clustering (MIMIC)


# Prerequisites for running code:
These instructions apply for Windows 10 x64. For testing on your own machine, you need to install the following libraries.

 ABAGAIL: https://github.com/pushkar/ABAGAIL
 Apache Ant: https://ant.apache.org/bindownload.cgi
 Java Development Kit: https://www.oracle.com/technetwork/java/javase/downloads/jdk10-downloads-4416644.html

Add Java and Ant to your windows environment and path variables. A helpful guide is found at: https://www.mkyong.com/ant/how-to-install-apache-ant-on-windows/
Once all of the prerequisites are installed, all of the methods are run from the Windows Command Prompt

Getting Started on How to run the code:
Section1: Training Weights for Neural Network. This section will train a neural network on the phishing websites dataset using RHC, SA, and GA. These methods are compared to each other and to the same network structure trained using backpropagation.

Edit the following .java files to point them towards the correct PhishingDataset.csv file location. There are following 5 .java files which is my overall code.

phishing_rhc.java : This file is for seeing behaviour of number of iterations on Test and traing accuracy for RHC
phishing_sa_para_tuning.java : This file is for parameter tuning for Simulated Annealing
phishing_sa_val_iter.java : This file is for seeing behaviour of number of iterations on Test and traing accuracy for Simulated Annealing
phishing_ga_para_tuning.java : This file is for parameter tuning for Genetic Algorithm
phishing_ga_val_iter.java : This file is for seeing behaviour of number of iterations on Test and traing accuracy for Genetic Algortihm

Convert all .java files to .class files with the following code from the command prompt.
javac phishing_rhc.java
javac phishing_sa_para_tuning.java
javac phishing_sa_val_iter.java
javac phishing_ga_para_tuning.java
javac phishing_ga_val_iter.java

Move all .class files to the location ~\ABAGAIL\opt\test
Includes the 5 'phishing_' class files and the 2 '_Toy' class files


Running the Models (via command prompt):

cd ~\ABAGAIL
ant
java -cp ABAGAIL.jar opt.test.phishing_rhc
java -cp ABAGAIL.jar opt.test.phishing_sa_para_tuning
java -cp ABAGAIL.jar opt.test.phishing_sa_val_iter
java -cp ABAGAIL.jar opt.test.phishing_ga_para_tuning
java -cp ABAGAIL.jar opt.test.phishing_ga_val_iter

The model results (training times and neural network accuracies) are stored in .csv files located at ~\ABAGAIL\Optimization_Results

Part 2: Random Search Toy Problems
This section presents 2 toy optimization problems for which RHC, SA, GA are all used to maximize the function fitness.

Similar procedure needs to be followed as Section 1 for files TravelingSalesman_Toy.java and ContinuousPeaks_Toy.java

1. Traveling Salesman Problem - Highlights GA
java -cp ABAGAIL.jar opt.test.TravelingSalesman_Toy
2. Continuous Peaks Problem - Highlights SA
java -cp ABAGAIL.jar opt.test.ContinuousPeaks_Toy

The model results (training times and fitness function values) are stored in .csv files located at ~\ABAGAIL\Optimization_Results

For graphs:
I used excel to create all the graphs given in the analysis. The graphs along with results can be seen in various excel files submitted.
