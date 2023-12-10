# Sentiment Analysis and Topic Modeling for Tweets
## Overview
This Python script performs sentiment analysis and topic modeling on a dataset of tweets using the pysentimiento library and a pre-trained model (cardiffnlp/tweet-topic-21-multi). The analysis includes extracting sentiments and topics from the tweets and aggregating statistics based on retweets, favorites, and followers. 
### Sentiment Analysis


### topic modeling

## Dependencies
  - ***pysentimiento***
  - ***transformers***
  - ***numpy***
  - ***scipy***
  - ***google-colab***
  - ***pandas***
  - ***gspread***
  - ***gspread-dataframe***
  - ***matplotlib_venn*** (if using Euler diagrams)
    
Install the dependencies using:\
```pip install pysentimiento transformers numpy scipy google-colab pandas gspread gspread-dataframe matplotlib-venn```

## Usage
Install the required dependencies.
Authenticate with Google Drive using the provided code.
Load the tweet data from the Google Sheets 'all_tweets' worksheet.
Perform sentiment analysis and topic modeling on each tweet.
Aggregate statistics based on sentiments, topics, retweets, favorites, and followers.
Create and populate new worksheets with the analysis results in the 'sentiment_results' Google Sheets.

## Files
**sentiment_analysis.ipynb**: Jupyter notebook containing the code.
**sentiment_results.csv**: CSV file containing the final analysis results.

## Instructions
Open and run the Jupyter notebook sentiment_analysis.ipynb in a Google Colab environment.
Follow the instructions in the notebook to authenticate and load data.
Run the notebook cells to perform sentiment analysis and topic modeling.
View the generated sentiment_results.csv file for the final analysis.

## Note
Ensure that you have the required access to Google Sheets and Drive.
Adjust the script as needed for your specific use case and data.

## Future enhancement 
- Euler diagrams can better illustrate overlapping topics.
- There are several ways to interpret topic vs sentiment, but this project is not about those interpretations.
- There is no clear data provided, but the data can be cleaned so that better results can be obtained more quickly.
- Topic modeling cannot identify some topics, so it can be retrained to improve its performance.
