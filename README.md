# Sparkify_Project


## Table of Contents
1. [Installation](https://github.com/Olek-ua/Sparkify_Project/tree/testing#installations)
2. [Project Motivation](https://github.com/Olek-ua/Sparkify_Project/tree/testing#project-motivation)
3. [File Descriptions](https://github.com/Olek-ua/Sparkify_Project/tree/testing#file-descriptions)
4. [Results](https://github.com/Olek-ua/Sparkify_Project/tree/testing#results)
5. [Licensing, Authors, and Acknowledgements](https://github.com/Olek-ua/Sparkify_Project/tree/testing#Licensing,-Authors,-and-Acknowledgement)

## Installations
You would need to install some of the standard data analysis & viz liabraries:

- numpy
- pandas
- matplotlib

and for data modelling we will use only:

- pyspark

The easiest way to install package is using `pip`

`pip install -U <package name>`

or `conda`:

`conda install -c conda-forge <package name>`

make sure to replace `<package name>` with actual package name, like:

`conda install -c conda-forge pyspark`

## Project Motivation

In this project I wanted to practice data manipulations as well as to explore ML
functionalities of PySpark library. To do that I've chosen Sparkify Project from
Udacity Nanodegree in Data Science. The project would require me to predict user
churn from a fictional company called Sparkify. Here are the key steps of this project

Also I wanted to compare how does Decision Tree performs against Logistic regression
performs for the churn prediction with the base for comparison would be precision.

I chose precision as the key metric with the idea that it's more important for us
to spot users who were mistakenly predicted to churn (False Negative) as for the
real world it's more important to prevent the churn, considering that sending
potential incentives to targeted users would not have significant cause.  

## File Descriptions

- **Sparkify.ipynb** - is the main Jupyter file. You can get my results by simply
running all lines in Jupyter notebooks. Beware that you may need to allocate some
extra memory on your machine, I used 15GB when setting up a spark session.

- **Train_onetag_small.json.zip** - zipped json file with the raw data. You would
need to unpack and save it in the project root folder.


## Results

Please check my [Medium post - Predicting user churn with PySpark](https://medium.com/@oleksandr_49102/predicting-user-churn-with-pyspark-4bdbed544cfc) for full discussion of the project.

Here is the quick summary of what we've found in this project:

 - _My Decision Tree model would perform better for user churn prediction in Sparkify platform_

 - _However I still did not find the result of 0.5 recall for Decision Tree model satisfactory._

- _Low recall result may be the reason of imbalanced data set with few target variables (~10%)_

- _The model is more likely to perform well on the full data set_

## Licensing, Authors, and Acknowledgements

The content of this repository is licensed under a [Creative Commons Attribution License](https://creativecommons.org/licenses/by/3.0/us/)
