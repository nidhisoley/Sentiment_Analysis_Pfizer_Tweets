# Sentiment Analysis for Pfizer Vaccine Tweets
## Data source
This project will focus on finding the sentiment of tweets concerning the Covid vaccine produced by Pfizer. Understanding the sentiment around the Pfizer vaccine will be helpful in understanding how the public feels, and indicate how receptive they are in taking the vaccine. To do this I will use an unannotated twitter dataset from Kaggle and perform an NLP Sentiment Analysis with a combination of various techniques. Can be found here: https://www.kaggle.com/datasets/gpreda/pfizer-vaccine-tweets?resource=download

## Hypothesis and Method
I performed the preprocessing of the tweets to get cleaner text and then performed some exploartory data analysis. The analysis helped me identify what were top hashtags, locations of tweets, number of tweets by date, etc. Then to perform sentiment analysis I used, VADER(Valence Aware Dictionary and sEntiment Reasoner) which is a lexicon and rule-based sentiment analysis tool that works especially well with social media texts. VADER is unique because it gives us polarity scores and can give us the intesity of the positive or negative tweet. VADER is able to not only map positive and negative words to the correct sentiment, but uses the context of the surrounding words to understand the tweets true sentiment. A person might tweet,"did not love", and VADER will classify it as negative, and not be confused by the positive word 'love'. This shows that VADER has been trained to better classify nuance in text. For this reason it works better for social media commments than a traditional Lexicon Word Counter. I also analysed how sentiment has looked over time.
Further, after identifying the location with highest number of tweets, I stratify the data to that location and see the sentiments of tweets and most common words used by the people of those locations.

## Conclusion
- There were 4197 unique tweets by the users all over the world about vaccine.  Top location of the users were London, India, and Singapore. Maximum users were unverfied. The most common hashtags were pfizerbiontech, covid19, covidvaccine. The analysis for the tweets by date suggestes that people tweeted the most in the period of Jan 2021 to April 2021, which is the period just after the Pfizer Disclosure notice came out. 
- The setiment analysis of the tweets indicates that the majority of the tweets were positive, with only 12.5% being negative. 
- The sentiments changed over time, people tweeted more positive tweets initially in the year and then there was a drop after May 2021, then there was a sudden increase in positive tweets in Oct-Sept 2021 which later dropped by the end of the year. The negative tweets were high in the intial months of the year and then remained more or less constant through out the year. 
- The major words used by the people for psoitive sentiments were success, created, vaccine, and daikon (because some folks suggested daikon paste can treat cytokine). The negative word cloud has words like death, side effect, first, stop, second, vaccine. 
- When I focused on users of London (location with highest tweets) I found that majority of sentiments were positive, with only 17% being negative. Most common words used by these people were pfizerbiontech, vaccine, first, got, done, thank.

I have added the pdf version of the code, because of the dynamic rendering problem of plotly on github.

Citation: Hutto, C.J. & Gilbert, E.E. (2014). VADER: A Parsimonious Rule-based Model for Sentiment Analysis of Social Media Text. Eighth International Conference on Weblogs and Social Media (ICWSM-14). Ann Arbor, MI, June 2014.
