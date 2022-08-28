# News Headline Sentiment Analysis

## Intro
The purpose of this project is to perform a sentiment analysis of news headlines to determine whether they are satirical or not. Given the current highly developed media in human society, sentiment analysis is now widely used in stock forecasting, economic forecasting, psychological guidance, etc.

## Methods
1. Use LSTM with Glove and W2V.
2. Use pretrained Bert.

## Data Description
Raw Data is a dataset collected from kaggle: https://www.kaggle.com/datasets/rmisra/news-headlines-dataset-for-sarcasm-detection
| Variable | DataType | Detail |
|--------|--------|--------|
| `headline` | Text | the headline of the news article |
| `article_link` | Text | link to the original news article. Useful for collecting supplementary data |
| `is_sarcastic` | Numeric | 1 if the record is sarcastic otherwise 0  |
