# Workflow Analysis for Social Media & Form Sentiment Analyzer

## Description
This workflow collects tweets mentioning 'strapi' or 'n8n.io' every 30 minutes and also accepts form submissions via a webhook. It analyzes the sentiment of both sources using Google Cloud Natural Language API, filters out retweets and outdated tweets, and stores only positive sentiment content in a Strapi CMS.

## Input Details
The workflow is triggered either by a scheduled interval (every 30 minutes for tweets) or by a POST webhook request containing form submission data.

## Process Summary
First, it fetches recent English tweets matching specific keywords and simplifies their structure. It filters out retweets and tweets older than 30 minutes. Separately, webhook form submissions are simplified. Both tweet and form content are sent to Google Cloud Natural Language for sentiment analysis. Only items with positive sentiment scores (above 0.3 for tweets, 0.4 for forms) are stored in Strapi as new posts.

## Output Details
Positive sentiment content from tweets and form submissions is stored as new entries in the Strapi CMS 'posts' content type.

## Tags
twitter, sentiment analysis, strapi, webhook, google cloud natural language, social media monitoring, form processing
