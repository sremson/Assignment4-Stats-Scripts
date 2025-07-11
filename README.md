# Assignment 4 Readme

## Setting up the environment
First I created a new environment to be able to complete this assignment. I only installed conda bioforge and jupyterlab, so I expect to be updating my environment consistently throughout this assignment to be able to complete the tutorial.

I used .gitignore to ignore all the .ipynbcheckpoint/ folders.

Upon looking at my environment file, I'm realizing there are a tonnnnn of dependencies there that I didn't mean to add myself. Not sure how they really got there as I created the environment in the terminal. I manually had to add pandas, scipy, matplot, and seaborn. I decided to delete all of the excess dependencies and add numpy as well.

## Beginning the Stats in Python Tutorial

- We want to use python for this because it makes powerful pipelines
- will be storing and manipulating data in a file called pandas.datafrome
- I downloaded the csv file and had pandas read it into a table
- it is pretty cool how well python can manipulate this data
- use "groupby" to split a dataframe on values of categorical variables

The mean for Females VIQ is 109.45 and the mean for Males VIQ is 115.0. The mean for all groups VIQ is 115.25. There were 39 participants in the study. 

## Plotting Data

- some of this data line is outdated. I had to look up how to translate this to an updated line of code, which involved using scatter_matrix instead of plotting
- i also made the csv file a readable dataframe to be able to make my plots
- i am having an extremely hard time getting this code to work. the plot is simply not showing up the way i want it to.
- i'm not entirely sure why the MRI/Height/Weight plot is not working the way the second plot is. For now i'm going to ignore it and move on.

## Hypothesis testing

- after running a one sample t-test, the p-value is 10^-28. this means that the mean of the population of VIQ is not 0.
- the result of the two sample t-test is a p-value of 0.44.
- the p-value from the repeated measures test is 0.08, and a 1 sample t-test on the difference gives the same value.
- the p-value as a result of a wilcoxon signed-rank test is 0.107.
- when doing the exercise, the p value for the difference between weights in males and females is 2^-5.
- 