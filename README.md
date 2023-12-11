# Sentiment Analysis and Topic Modeling for Tweets
## Overview
This Python script conducts sentiment analysis and topic modeling on a dataset of tweets, utilizing the pysentimiento library and a pre-trained model (cardiffnlp/tweet-topic-21-multi). The analysis involves extracting sentiments and topics from tweets, followed by aggregating statistics based on retweets, favorites, and followers. Approximately **~94.53%** accuracy was achieved for this specific use case.\
**Accuracy:0.9453422437803131** (mean prob score for the applied models)
### Sentiment Analysis
The sentiment analysis is performed using [pysentimiento](https://github.com/pysentimiento/pysentimiento), a powerful tool built for sentiment analysis tasks. This tool utilizes a pre-trained model trained on a diverse set of approximately 40,000 tweets. Specifically, it relies on [BERTweet](https://github.com/VinAIResearch/BERTweet), a RoBERTa model fine-tuned for sentiment analysis on English tweets. The choice of these tools ensures accurate and context-aware sentiment analysis. For more details, you can refer to the [Hugging Face model page](https://huggingface.co/finiteautomata/bertweet-base-sentiment-analysis).
### topic modeling 
The topic modeling leverages [cardiffnlp/tweet-topic-21-multi](https://huggingface.co/cardiffnlp/tweet-topic-21-multi), a state-of-the-art [Transformer](https://huggingface.co/learn/nlp-course/chapter1/4?fw=pt) model. This model, built upon [TimeLMs](https://github.com/cardiffnlp/timelms), is trained on a substantial dataset of around ~124 million tweets and fine-tuned for optimal performance in topic extraction tasks. For a detailed understanding, you can refer to the [base paper](https://arxiv.org/abs/2209.09824) associated with this model.

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
    
Install the dependencies using:
```
pip install pysentimiento transformers numpy scipy google-colab pandas gspread gspread-dataframe matplotlib-venn
```
## Usage
1. Install the required dependencies.
2. Authenticate with Google Drive using the provided code.
3. Load the tweet data from the Google Sheets 'all_tweets' worksheet.
4. Perform sentiment analysis and topic modeling on each tweet.
5. Aggregate statistics based on sentiments, topics, retweets, favorites, and followers.
6. Create and populate new worksheets with the analysis results in the 'sentiment_results' Google Sheets.

## Files
**sentiment_analysis.ipynb**: Jupyter notebook containing the code.\
**sentiment_results.csv**: CSV file containing the final analysis results.

## Instructions
1. Open and run the Jupyter Notebook sentiment_analysis.ipynb in a Google Colab environment.
2. Follow the instructions in the notebook to authenticate and load data.
3. Run the notebook cells to perform sentiment analysis and topic modeling.
4. View the generated sentiment_results.csv file for the final analysis.

## Note
Ensure that you have the required access to Google Sheets and Drive.
Adjust the script as needed for your specific use case and data.\
**Results and base data used are found in the [Excel_sheet](https://github.com/ShreehariA/twitter-data-analysis/tree/main/Excel_file) folder.**

## Future Enhancement 
- Consider enhancing the visualization by incorporating Euler diagrams to illustrate overlapping topics more effectively.
- Explore different interpretations of topic vs. sentiment, although this project may not focus on those interpretations.
- Clean the data for better and quicker results.
- Retrain the topic modeling model to improve its performance, especially in identifying certain topics.

