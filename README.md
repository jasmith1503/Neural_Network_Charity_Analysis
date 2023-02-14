# Neural Network Charity Analysis
Module 20 Challenge - Supervised Machine Learning

## Resources
Operating Platform: Windows 11 Pro - Build 22621 [Buy Windows 11 Pro](https://www.microsoft.com/en-us/d/windows-11-pro/dg7gmgf0d8h4?rtc=1)</br>
IDE Software: [Jupyter Notebook](https://jupyter.org/) Verison 6.5.2 ()</br>
Python Kernel: 3.7.13</br>
Completed Jupyter Notebooks: [AlphabetSoupCharity](AlphabetSoupCharity.ipynb)</br>
Resource files: [Charity Data](/Resources/charity_data.csv)</br>

## Overview
Alphabet Soup, a fictious non-profit fund raising company is trying to determine which canidates will be successful if funded. Using neural networks and a variety of techniques I attempt to create a Machine Learning module to find the best fit. The dataset contains 34,000 organizations that have received funding from Alphabet Soup over the years.


## Overview of the analysis & Data Preprocessing: 
The overview is to take the data found inside the csv charity file and ingest the data into a Pandas dataframe. From there a few columns are removed ['EIN', 'NAME'] because they do not add into the overall feature data. The specific columns to target for the machine learning module are ['IS_SUCCESSFUL']. Additional cleanup was done on the data found in the below two columns
[‘CLASSIFICATION’] 
[‘APPLICATION_TYPE’]
The reason for the changes was due to the fact of types of results found inside each column, Application_Type had 17 unique results and Classification had 71 components. In order to use OneHotEncoder this list should be trimmed down to about 9 results. 

Compiling, Training, and Evaluating the Model: 
For my first run 
