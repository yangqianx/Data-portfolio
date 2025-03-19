# Master-Thesis-Project
Explore weight loss discussions and sentiments on Reddit

# Overview
This study investigates the weight loss discussions and sentiments on Reddit during the COVID-19
pandemic. This study collected and analyzed a dataset containing 35,384 posts from March 2019 to March
2021 in the loseit subreddit. To compare and explore how discussions and sentiments changed within this
weight loss subreddit, the analysis utilized two unsupervised machine learning methods, topic modeling
and sentiment analysis, to explore the evolution of the topics and emotional expressions of weight loss
discussions over time. By employing topic modeling (LDA), the study identified 16 topics within five
categories of weight loss discussions: Weight Management, Diet, Physical Exercise, Emotions and Support,
and Appearance. However, topic related weight loss as well as upstream and downstream such as Weight
change (T2), Calorie tracker (T3), Motivation (T4) and Workout plan (T15) varied over time. Furthermore,
Sentiment analysis indicated that discussions in the loseit subreddit are mainly positive rather than negative.
There was a slight increase in negative sentiments and a decrease in positive throughout the study period.
Emotion analysis indicates the complexity of the emotion dynamic in weight loss discussions. Moreover,
users in this weight loss subreddit frequently expressed positive emotions, such as anticipation, and negative
emotions, such as fear. However, the sentiments and emotions varied significantly among most topics.
These findings reveal how social media affected netizens' attitudes and behaviour on this topic and how it
changed during this global crisis. While the study noted significant sentiment changes in some topics across
the two time periods in this weight loss subreddit, it remains cautious about concluding the impact of the
pandemic in weight loss discussion on social media. Further study could explore a more extended period
in multiple subreddits or social media platforms to conclusively link these trends with the pandemic's effect.

# Data
loseit_submissions.zst : The historical dataset contain original post data of 'r/loseit'.  
loseit_submissions_2019_2021_ids.txt: The IDs files from 2019 to 2021 exported from the historical dataset.  
Submissions.csv: This file contains the post content and its metadata collecting from Reddit.  
Cleaned submissions.csv:This file contains submission dataset that has been initially cleaned.  
Processed_lda.csv:The file contains Cleaned submissions that has been text cleaning and preprocessing for LDA
algorithm.  
Processed_vader.csv:The file contains Cleaned submissions that has been text cleaning and preprocessing for
VADER analysis.  
Processed_nrc.csv:The file contains Cleaned submissions that has been text cleaning and preprocessing for
NRC-EIL analysis.  
lda_submissions.csv:This file contains the results of LDA analysis of each post and related metadata.  
vader_submissions.csv: This file contains the result of VADER sentiment analysis and weighted sentiment score
of each post with related metadata.  
nrc_submissions.csv: This file contains the result after applying the NRC-EIL analysis (eight emotions and
corresponding scores) of each post with related metadata.  

# Package

This project requires the following Python packages:  
Core: os, sys, json, csv, datetime, logging  
Scraping: praw, pandas, BeautifulSoup, re  
NLP: nltk, spacy, gensim  
Stats & Modeling: numpy, scipy, statsmodels  
Visualization: matplotlib, plotly  
Other: zstandard, ast  
