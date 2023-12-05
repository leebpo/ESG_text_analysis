# ESG_text_analysis
*Richard Shum, Christy Fang, Hedy Sun, Jo Lee*

## Introduction

This is a text analysis project on ESG reports that explores company priorities. ESG reports are documents outlining a company’s goals and performances in the areas of environmental, social, and governance practices. We want to explore a company’s values and what topics they focus on, as well as whether these values are shared across the industry. <br>

## Data

We picked 5 industries for our data which includes Food, Technology, Media, Retail and Airlines and we picked 3 companies for each industry. We have downloaded 15 ESG pdf reports from 2022-2023 from companies' respective websites and stored them in the `Reports/` folder. <br>

We also have a csv file `ESGword.csv` which hold keywords and key bigrams that relate to environmental, social and governance categories. We made this csv by first creating a default list using ChatGPT then iterativly pulling word frequencies from the report texts to add more common phrases that fell into those categories and maximize these lists in the csv as much as possible.

## Code

The code in main.ipynb uses `PyPDF2` Python module to extract the text from the pdf files and store them in text files. We also made text files for each industry which just aggregated all the text from the reports of companies in that industry. We stored these txt files in the `Textfiles/` folder. <br>
We ran three different analysis: 
1. Unigrams
   a) Word clouds for each company as well as each industry
   b) Pie charts on environmental, social, and governance words found for each company and industry
   c) Printing top 20 most frequent words for each company
3. Bigrams
   a) Pie charts on environmental, social, and governance bigrams found for each company and industry
   b) Printing top 20 most frequent bigrams for each company
5. TF-IDF
   a) Heatmap of frequent terms for each industry

## Presentation
For the presentation of this project, we manually created bar graphs using the numbers displayed on the pie charts for the sake of saving space on slides. 
