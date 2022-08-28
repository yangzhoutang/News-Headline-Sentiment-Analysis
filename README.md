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

## Conclusion
The best result is from Bert, with about 0.81 accuracy score. Due to the nature of Bert as a transformer pretrained by an insanely large dataset, it costs almost 10x time than LSTM+W2V+GLOVE. However, LSTM with W2V and Glove can also hit 0.78, which is a good choice for quick sentiment analysis when we don't have too much time to cost.
