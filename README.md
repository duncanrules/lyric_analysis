# Text Mining Song Lyrics
Using text mining techniques on song lyrics to predict success
- - - -

## Hypothesis

Our hypothesis is that the emotion, sentiment, and topics of a song’s lyrics influence its performance on the Billboard Top 100 chart. More specifically, we believe that supervised learning models that include a song’s lyric features can perform better than comparable models that only use the song’s metadata, such as title, artist, and year released. For example, we may find that sad songs released by a certain artist, or that songs with topics pertaining to love are likely to place on the Billboard chart.

## Data

The data was obtained from multiple Kaggle datasets of songs and their lyrics; the first was a dataset in which the host took the year end Billboard charts and scraped song lyrics websites. The second and third are more exhaustive song lyric datasets scraped from similar sites, but include both songs that were present on the Top 100 chart and those that were not. By combining these datasets, we can get a large amount of songs and their lyrics, as well as labels of “success” as determined by whether or not they made the chart. Since the Billboard Top 100 chart ranges from 1964 to 2015, there will likely be a time series bias while working with the data and recency bias with more songs being released closer to current day. 

[[1]](https://www.kaggle.com/rakannimer/billboard-lyrics)[[2]](https://www.kaggle.com/mousehead/songlyrics)[[3]](https://www.kaggle.com/artimous/every-song-you-have-heard-almost)

## Planned Methods

Data preparation will be done using topic modelling and sentiment analysis. We will test LDA, KNN, SVM, Naïve Bayes and neural nets if the data and architecture allows. We will choose the optimal solution based on our training data metrics. These methods require very little to no labelled data and classify the response variable based on the inherent relationships the predictor variables group by. These methods have been applied to text mining with varying rates of success but we feel applying text mining to predict Billboard Top 100 songs solely using lyrics is a novel approach in itself.
