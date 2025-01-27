# **Active-Learning-for-Practical-Identifiability**

This repository contains the code for the paper “Efficiently Establishing Practical Identifiability via Active Learning”.

**Overview**

The code is written in R notebook format and can be run in RStudio. It demonstrates how to efficiently establish practical identifiability through active learning in our case study model, as discussed in the associated research paper *“Efficiently Establishing Practical Identifiability via Active Learning”*.

**Getting Started**

	Download and open the R notebook files in RStudio.
	You can control the number of replications and iterations by modifying the parameters in the last row of both files.
	Example: trials(Replication, Iteration, 60)
	Replication: Number of replications to run
	Iteration: Number of iterations per replication
	60: A constant parameter (Our range for the time axis)

**Requirements**

	•	RStudio  
	•	Required the installication of RSTAN (Following link: https://mc-stan.org/rstan/)
