# ESG_text_analysis
Final Project for Fall 2023 course CSCI2349:Text Processing, taught by Professor Prud'hommeaux<br>
*Richard Shum, Christy Fang, Hedy Sun, Jo Lee*

## Introduction

This is a text analysis project on ESG reports. ESG reports are documents outlining a company’s goals and performances in the areas of environmental, social, and governance practices. We want to explore a company’s values and whether these values are shared across the industry. <br>

## Data

We picked 5 industries: Food, Technology, Media, Retail and Airlines. We picked 3 companies for each industry. We downloaded 15 ESG pdf reports from 2022-2023 from companies' respective websites and stored them in the `Reports/` folder. <br>

We also have a csv file `ESGword.csv` holding keywords and key bigrams that relate to environmental, social and governance categories. We made this csv by first generating a default list using ChatGPT then iterativly pulling word frequencies from the report texts to add more common phrases to maximize these lists as much as possible.

## Code

The code in main.ipynb uses `PyPDF2` Python module to extract the text from the pdf files and store them in text files. We also made text files for each industry which just aggregated all the text from the reports of companies in that industry. We stored these txt files in the `Textfiles/` folder. <br>
We ran three different analysis: 
* Unigrams
   1. Word clouds for each company as well as each industry
   2. Pie charts on environmental, social, and governance words found for each company and industry
   3. Printing top 20 most frequent words for each company
* Bigrams
   1. Pie charts on environmental, social, and governance bigrams found for each company and industry
   2. Printing top 20 most frequent bigrams for each company
* TF-IDF
   1. Heatmap of frequent terms for each industry

## Presentation
For the presentation of this project, we manually created bar graphs using the numbers displayed on the pie charts for the sake of saving space on slides. 
