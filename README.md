# Sentiment-Analyser-for-tweets

In this notebook, we intend to fetch all the tweets having a particular hashtag or keyword in them and ultimately, predict the underlying sentiment i.e. positive or negative which it represents based on its text content.

The tweets are extracted by hitting the Twitter API by accessing the [tweepy](http://www.tweepy.org/) library.

After extraction in bulk, it is saved into a text file. Only the required fields are then read out of this file and written into a csv file.

The text column for this tweets csv file is cleaned removing special characters like hashtags,urls,etc using **re**(regular expressions) and stopwords removed using **nltk** libraries.Any duplicated rows or null valued columns are also dropped from the data.

Finally, the [TextBlob](https://textblob.readthedocs.io/en/dev/) library to perform sentiment analysis on each cleaned Tweet. How positive or negative each tweet is about whatever topic we choose is stored into the csv file.

## Requirements:
- TextBlob
- tweepy
- pandas
- jsonpickle
- json
- csv
- re
- nltk
