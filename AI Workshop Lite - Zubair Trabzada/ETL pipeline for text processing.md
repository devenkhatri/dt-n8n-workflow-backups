# Workflow Analysis for ETL pipeline

## Description
This workflow fetches tweets containing the hashtag #OnThisDay, analyzes their sentiment using Google Cloud Natural Language API, stores the results in a PostgreSQL database, and sends a Slack notification for tweets with a positive sentiment score.

## Input Details
The workflow is triggered daily at 6 AM via a cron job and initially fetches tweets containing the hashtag #OnThisDay from Twitter.

## Process Summary
The workflow starts by fetching up to 3 tweets with the hashtag #OnThisDay from Twitter. These tweets are inserted into a MongoDB collection. The text from each tweet is then sent to Google Cloud Natural Language API for sentiment analysis. The sentiment score and magnitude, along with the tweet text, are formatted and stored in a PostgreSQL table named 'tweets'. Finally, an IF node checks if the sentiment score is greater than 0, and if so, sends a notification to a Slack channel; otherwise, it proceeds to a NoOp node.

## Output Details
The workflow stores enriched tweet data (text, sentiment score, and magnitude) in a PostgreSQL database and sends positive-sentiment tweet alerts to a Slack channel named 'tweets'.

## Tags
ETL, Twitter, Sentiment Analysis, Slack Notification, PostgreSQL, MongoDB, Google Cloud Natural Language, Cron Trigger
