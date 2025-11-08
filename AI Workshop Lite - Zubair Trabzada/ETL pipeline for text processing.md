# Workflow Analysis for Twitter Sentiment Analysis ETL and Notification

## Description
This workflow automatically fetches tweets, analyzes their sentiment using Google Cloud Natural Language, stores the data in MongoDB and PostgreSQL databases, and sends Slack notifications for tweets with positive sentiment.

## Input Details
The workflow is triggered daily at 6 AM by a cron schedule and then fetches recent tweets containing the "#OnThisDay" hashtag from Twitter.

## Process Summary
First, the workflow queries Twitter for tweets with the hashtag "#OnThisDay". Next, it inserts these tweets into a MongoDB collection. Then, the tweet text is sent to Google Cloud Natural Language for sentiment analysis. The sentiment score, magnitude, and tweet text are extracted and prepared. This processed data is then stored in a PostgreSQL database. Finally, a condition checks if the tweet's sentiment score is positive; if so, a Slack message is sent with the tweet details.

## Output Details
The workflow stores fetched tweets in MongoDB, processed tweets with sentiment scores in PostgreSQL, and sends conditional notifications to a Slack channel.
