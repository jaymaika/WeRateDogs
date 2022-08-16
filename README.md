# WeRateDogs Data Wrangling

## Dataset

The WeRateDogs data wrangling project focuses on cleaning of the data acquired from different sources. For this project, data was collected from three different sourcer; twiter in form of .json, a url to download the data stored in a TSV file and a basic .csv file format.


## Summary of Findings

After gathering the dataset, both manual and programmatic assessment was done on each of the dataframes. During this process, a number of observations on quality and tidiness were made:
There was an interesting point to note about some of the ratings extracted from the text. I noticed that some ratings had an aggregate of the number of dogs in the picture, for example, similar cases where a rating of 88/80 was given to a group of 8 dogs all together, meaning the individual rating for each dog is actually 11/10. This was corrected during the cleaning phase.

Quality
archive dataset
1. some records are retweets 
2. erroneous dog stage classification
3. some records don't have images
4. Inaccurate rating values. Some texts contain dates/values in the same format as the ratings which have then been mistaken for ratings.
5. Some columns have no values 

image dataset
1. non-descriptive column names

tweepy api dataset
1. retweet counts and favorite counts are objects instead of integers 
2. deleted tweets

Tidiness
1. Retweet count and favorite count should be part of the archive dataset.
2. The image dataset should be part of the archive dataset.
3. three different confidence score predictions and breeds(only one, ié the highest confidence score is required for this analysis) 




