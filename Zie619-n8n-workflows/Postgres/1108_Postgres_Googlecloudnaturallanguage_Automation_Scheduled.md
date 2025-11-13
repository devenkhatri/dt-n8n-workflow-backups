# Workflow Analysis for ETL Pipeline

## Description
This workflow is an automated ETL pipeline that processes data from Twitter and performs sentiment analysis using Google Cloud Natural Language, storing the results in a MongoDB database and sending notifications to a Slack channel.

## Input Details
The workflow is triggered by a Cron node at 6am every day and receives data from Twitter based on the #OnThisDay hashtag.

## Process Summary
The workflow starts by fetching tweets from Twitter using the #OnThisDay hashtag, then stores the tweets in a MongoDB database. The tweets are then analyzed using Google Cloud Natural Language to determine their sentiment score and magnitude. The sentiment scores are then used to determine whether the tweet should be sent to a Slack channel. If the score is higher than a certain threshold, the tweet is sent to the Slack channel.

## Output Details
The workflow produces a notification in a Slack channel with the tweet text, sentiment score, and magnitude, and also stores the tweet data in a MongoDB database.

## Tags
automation, etl, twitter, mongodb, google cloud natural language, slack, cron, sentiment analysis
