# Workflow Analysis for Production Workflow

## Description
This workflow monitors social media and form submissions, analyzes their sentiment, and stores positively-toned content in a Strapi CMS.

## Input Details
The workflow is triggered either every 30 minutes to search for relevant tweets or by an incoming webhook containing form submission data.

## Process Summary
The workflow is triggered either on a schedule to search for tweets or by a webhook for form submissions. For tweets, it filters out retweets and old posts, then extracts content, author, creation date, and URL. For form submissions, it extracts content and author. Both pathways analyze the sentiment of the extracted text using Google Cloud Natural Language. Based on predefined sentiment thresholds, only content with positive sentiment is allowed to proceed.

## Output Details
The workflow creates new entries ("posts") in a Strapi CMS for tweets and form submissions identified as having a positive sentiment.

## Tags
twitter, sentiment analysis, Strapi, webhook, scheduled, content management, automation, n8n
