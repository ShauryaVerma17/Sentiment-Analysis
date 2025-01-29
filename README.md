# Sentiment-Analysis

Repository for keeping POCs related to sentiment analysis

## Pre-requisites 

To run this repo using VS code you will need to first run a few commands. Here are the steps :

1. Once you've cloned the repository open up VSCode and open the project folder.
2. Start the terminal and run the following commands :
   #### 1. Creating a virtual environment
       python -m venv .venv
   #### 2. Running the virtual environment
       .venv\scripts\activate
   #### 3. Installing all the required libraries into the virtual environment (Make sure virtual environment is enabled and you are in the main parent folder of the project)
       pip install -r requirements.txt

## Notebooks in the repo (src folder)

### BagOfWordsMethod

This notebook builds up a POC on performing sentiment analysis using the python library called VADER.

### EncoderOnlyTransformerMethod

This notebook builds up a POC on performing sentiment analysis using Encoder-Only Transformer based models like BERT, RoBERTa or DeBERTa by utilizing the transformers library from huggingface.

### PerformanceComparison

After developing an understanding of how the two methods work, we compare their performances on a predefined template dataset. 

## Data used for analysis (data folder)

### AmazonReviews.csv

This file contains 25000 amazon reviews along with the star ratings used for analysis in the PerformanceComparison notebook.

### AnalysisResults.csv and AnalysisResults.xlsx

These files both contain the result of running sentiment analysis on the above dataset using Vader and Encoder Only Transformer approach.

### AnalysisOfAnalysis.txt

This file contains the conclusion drawn from the results of the comparison. It shows the avg score given by both approaches for each star rating.
