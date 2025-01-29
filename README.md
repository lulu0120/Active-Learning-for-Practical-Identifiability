# **Active-Learning-for-Practical-Identifiability**

This repository contains the code for the paper “Efficiently Establishing Practical Identifiability via Active Learning”.

**Overview**

The code is written in R notebook format and can be run in RStudio. It demonstrates how to efficiently establish practical identifiability through active learning in our case study model, as discussed in the associated research paper *“Efficiently Establishing Practical Identifiability via Active Learning”*.

**Requirements**

	•	RStudio  
	•	Required the installication of RSTAN (Following link: https://mc-stan.org/rstan/)

**Getting Started**

	Download and open the R notebook files in RStudio.
	You can control the number of replications and iterations by modifying the parameters in the last row of both files.
	Example: trials(Replication, Iteration, 60)
	Replication: Number of replications to run
	Iteration: Number of iterations per replication
	60: A constant parameter (Our range for the time axis)

**Output Explaination**

Calling A = trials(Replication, Iteration, 60) returns an object A, which contains multiple result components.

	Each replication result can be accessed using A[i][j], where:
	•	i refers to the type of result (from 1 to 5, as listed below).
	•	j refers to the specific replication number.

The outputs for i follow the order below:

	1.	estimated_params: The estimated model parameters (Maximum Likelihood Estimator) based on collected data.
	2.	observations: The data collected by the algorithm.
	3.	obs_locations_df: A data frame indicating the locations of collected observations.
	4.	pl_check: A validation check for practical identifiability using profile likelihood.
	5.	bounds: The profile likelihood confidence intervals based on existing data.

