# Udacity Data Wrangling & Scraping Project: WeRateDogs Twitter Data
## by Ayse Isin Budak
 
 
## Introduction
***
This project is completed under the Udacity Data Analyst Nanodegree program and focused on performing data scraping and wrangling.
In this project, I scraped the Tweet archive of the Twitter WeRateDogs account and merged it with .tsv and .csv files for further analysis,
Please note that cleaning and analyzing is not exhaustive but limited to 10 steps requested by Udacity.

##### `Pre-requisite Python packages`
<li>csv
<li>pandas
<li>requests
<li>os
<li>io
<li>numpy
<li>tweepy
<li>json
<li>timeit
<li>matplotlib.pyplot
<li>seaborn


## A. Gather
***
##### `tweet_json1.txt`
I created this file by scraping and using the Tweepy API. Favorite and retweet counts for each tweet id in twitter-archive-enhanced.csv is fetched.

##### `twitter-archive-enhanced.csv`
The WeRateDogs Twitter archive data wrangled and provided by Udacity.

##### `image_predictions.tsv`
Tweet image predictions fetched from Udacity's servers.




## B. Assess
***
<li>Initial visual analysis (Inspecting samples for anomalies.)
<li>Collecting information on data using panda (e.g. data types, value counts, null values)
<li>Advanced data quality/tidiness analysis using pandas. (Ex: Irrelevant data exclusion)
    
There were several issues found and classified in two groups below: quality and tidiness.
## C. Clean
***
### Quality
##### `archive` table 
1. Retweets are removed.
2. Erroneous data types found: timestamp column is converted to timestamp. The nominator and denominator are converted to integers.
3. Lower case words replaced with an empty string in the name column as they are not real names e.g. A, an the.
4. There are outliers in the rating numerator. Some of them are because of multiple occurrences of the pattern \d+\/\d+.
   Outliers due to multiple occurrences of the pattern \d+\/\d+ are corrected.  
5. Rating numerator column has some exceptionally high values which lead to exceptionally high ratings which can be inaccurate.
   Some of the exceptionally high rating numerators are due to non-integer entries. Those entries are corrected.
6. Source column had the HTML tags. Removing tags, 3 different data sources become readable

##### `image prediction` table
7. p1, p2, p3 written in both uppercase and lowercase. Lower() function is used to standardize data.


### Tidiness
##### `archive` table
8. Columns for dog stages are untidy. Single column is created by using melt() function.

##### `image prediction`  &  `df_tweet_json` table
9. and 10. These data sets are part of the same observational unit as the data in the archive. Three tables are joined. 



##### `twitter-archive-enhanced.csv`
The WeRateDogs Twitter archive data wrangled and provided by Udacity.

##### `image_predictions.tsv`
Tweet image predictions fetched from Udacity's servers.


```python

```
