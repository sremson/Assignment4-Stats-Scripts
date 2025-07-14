# Assignment 4 Readme- Python Statistics Walkthrough

The purpose of this assignment is to understand using Python for statistical analysis at a deeper level! This repo will contain my jupyterlab notebook where I did all the code and examples, as well as this readme. Here, I tried to explain a bit what the purpose of each test was and include my results and parameters, as well as thoughts that I had while I was going through the assignment. This was great practice for applyin common statistical and plotting techniques, I'm sure I can reference this in the future when looking to do data analysis in my lab.

## Source

I followed the tutorial from this website:
https://scipy-lectures.org/packages/statistics/index.html

## Getting started

### Cloning the repository

I made my repo and added the gitignore. I then cloned the repo here.
https://github.com/sremson/Assignment4-Stats-Scripts

### Setting up the environment
First I created a new environment to be able to complete this assignment. I only installed conda bioforge and jupyterlab, so I expect to be updating my environment consistently throughout this assignment to be able to complete the tutorial.

I used .gitignore to ignore all the .ipynbcheckpoint/ folders.

Upon looking at my environment file, I'm realizing there are a tonnnnn of dependencies there that I didn't mean to add myself. Not sure how they really got there as I created the environment in the terminal. I manually had to add pandas, scipy, matplot, and seaborn. I decided to delete all of the excess dependencies and add numpy as well.

bash stats-env.sh

The /notebook was not working for me because jupyterlab does not like "/".

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

## Linear models, multiple factors, and analysis of variance

- no we are testing the hypothesis that y is a linear function of x
- y= x * coeff + intercept + e
- For the first exercise, the paramaters are as follows:
- int: -5.53, x: 2.94
- next i did a comparison between IQ of male and females using a linear model and got these parameters:
- int: 109.45, Gender(T.male): 5.8
- now we are comparing different types of IQ with a long form table
- multiple regression time! I imported the new CSV file
- the f test result gave a p value of 0.07
- When testing the difference between males and females for VIQ, we can see there is no difference (the hypothesis is not supported)

## Using seaborn for statistical exploration
- i imported the example data (wages.txt)
- i then used seaborn to make a scatter matrix looking at all of the variables, then plotted the categorical variables as a hue
- i the did a regression plot looking at just single variables. this model, however, includes outliers, so we would have to do a robus model in order to get rid of those

## testing for interactions
- had to adjust the names of the variables to correctly reflect what the column labels are
- the take home messages here:
- hypothesis testing/p values give you the signficance of the statistical difference
- formulas help you express connections between your data
- visualizing data helps give more insight
- conditioning the data can allow for different interpretation

## License

This repository is itended for educational use only.

## Acknowledgements

Based on exercises from:
https://scipy-lectures.org/packages/statistics/index.html
The SciPy Lecture Notes authors
Also the best intructions from Dr. Mike Freitas :)
