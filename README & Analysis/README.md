# Assignment_1

This is the assignment #1 for the class "Introduction to Data Science". I tried to find out whether "news is a downer" or not.

###Methodology###
I used the Twitter API to download 6000 tweets from 10 media sources (600 tweets each). The selection of the media sources are based on the popularity (they are all most followed accounts) and relevance (I excluded popular accounts such as "TheEconomist" and "FT" for their high emphases on economics/finance, similarly, I have replaced "BBCBreaking" with "BBCworld" for the reason that "BBCworld" has a more general and traditional coverage rather than emphasize only on breaking news).The 10 Media Source that I used are **New York Times, NPR News, Washington Post, CNN, Fox News, Huffington Post, BBC World News, Reuters, ABC News and Wall Street Journal.**

I then analysized the tweets using r, with the main structure similar to what has been taught on Dr.Barbera's workshop. Using a lexicon from Neal Caren of positive and negative words, results from each media accounts were shown. I further conducted an hypothesis test about the difference of the mean of the positive and negative group, and found that under convential significance level we would reject the null hypothesis that news is a downer.(p=0.0206)

A cautinary note that the tweets that I gathered from API is up-to-date so the timing of getting the data might influence the analysis output. I have tried to run the code and to get data several times (during different time of a day, and in different day of the week) and found the statistical significance remain unchanged.

###Findings###
The main findings are discussed below with charts and graphs.

###Sentiment Analysis Outputs###
![Alt Text](https://github.com/yuqiliao/Assignment_1/blob/master/Sentiment%20Analysis%20Results.png)
![Alt Text](https://github.com/yuqiliao/Assignment_1/blob/master/Comparison%20Chart.png)

- Neutral words are around 50% of the tweets for each account.
- Negative words are generally more than positive words in terms of percentage.
  - Besides New York Times, NPR News and Wall Street Journal, the percentage of negative words are bigger than positive words for other accounts.
- The differences between the percentage of positive words and negative words vary across different accounts
  - The percentage of negative words from Fox News, BBC World, Reuters and ABC News are 10 percentage points more than their positive words

###Statistical Test###
![Alt Text](https://github.com/yuqiliao/Assignment_1/blob/master/Ttest%20Output.png)

The t-test output rejects the null hypothesis that there is no difference between the mean percentage of positive words and that of negative words.(P=0.0206). **In other words, the difference between the two categories are statistically significant, indicating that the "hard news" are highly likely to be about "bad(negative) news".**
