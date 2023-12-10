# About the Excel sheet
Welcome to the Tweet Analysis project! This analysis focuses on tweets related to research, aiming to extract valuable insights and trends from the data.\
This file contains plenty of sheets so let me explain a bit there are 2 parts: the **base data** that is used in this analysis and the obtained **results** in separate sheets.

## Results
### analysis_added
The "analysis_added" sheet presents raw data obtained after sentiment analysis and topic modeling. The "prob_score" column represents the probability score, indicating the confidence level of sentiment predictions. 3 new columns are added in as a result of this project
- sentiment
- topic
- prob_score
- Example data snippet
~~~
| sentiment | topic | prob_score |
|-----------|-------|------------|
| POS       | ...   | 0.90       |
| NEG       | ...   | 0.85       |
| NEU       | ...   | 0.82       |
~~~
### sentiment_analysis
Explore the correlation between sentiments and engagement metrics **(Retweets, Favorites, Followers)**. Visualizations, such as heat maps and bar graphs, offer a comprehensive view of sentiment trends.\
Example Graph\
<img width="359" alt="Retweets" src="https://github.com/ShreehariA/twitter-data-analysis/assets/122812415/f19c6891-5198-49da-95aa-c8d8ee4fd52e">
### topic_analysis
Understand how different topics relate to engagement metrics. This sheet provides insights into the impact of various topics on **Retweets, Favorites, and Followers**.\
Example Graph\
<img width="329" alt="topic_retweets" src="https://github.com/ShreehariA/twitter-data-analysis/assets/122812415/6958c654-63a5-483d-9143-680415d27774">
### overlapping
Discover relationships between **sentiments** and **topics**, analyzing trends in the combinations of sentiments and topics within research-related tweets.\
Example Graph\
<img width="482" alt="sentement overlaping" src="https://github.com/ShreehariA/twitter-data-analysis/assets/122812415/ed183bdf-716e-4158-a7f6-631822cc861a">

## Base data
### All Tweets
The "All Tweets" sheet contains data directly from the API. Tweets are filtered to include only those related to research, ensuring the analysis focuses on relevant content.
### Others
Other sheets are the initial analysis that is done on the data to get a better picture of the data some important sheets that are interesting to look at are as follows:\
**Hashtags**: Gain a comprehensive list of hashtags used in the tweets, revealing popular themes within the research community.\
**World map**: Explore the geographical distribution of tweets and tweet density, providing insights into the global reach of research-related content.\
<img width="457" alt="world map" src="https://github.com/ShreehariA/twitter-data-analysis/assets/122812415/7b8e03d7-1e10-44c9-8e05-7354f45633bd">
