# Workflow Analysis for Content Sentiment Analysis and Storage in Strapi

## Description
This workflow automatically monitors Twitter for specific keywords and processes incoming form submissions. It analyzes the sentiment of the text content using Google Cloud Natural Language and stores positively-rated content in a Strapi CMS.

## Input Details
The workflow is triggered either by a scheduled interval every 30 minutes to search Twitter for tweets or by a webhook receiving a POST request with form submission data.

## Process Summary
The workflow either searches Twitter for "strapi" or "n8n.io" tweets every 30 minutes or processes incoming form submissions via a webhook. For tweets, it filters out retweets and old posts, then extracts relevant details like content, author, and URL. Both tweet content and form submission content are sent to Google Cloud Natural Language for sentiment analysis. The sentiment analysis results are merged with the original data. Finally, it checks if the sentiment score is positive (greater than 0.3 for tweets, 0.4 for form submissions). If positive, the content is stored in Strapi.

## Output Details
The workflow stores processed tweets with positive sentiment and form submissions with positive sentiment as new "posts" in a Strapi CMS.
