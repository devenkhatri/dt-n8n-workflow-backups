# Workflow Analysis for Production Workflow

## Description
Production-ready workflow: Production Workflow. This workflow has been optimized for production use with comprehensive error handling, security, and documentation.

## Input Details
The workflow is triggered either every 30 minutes to search for tweets or by a POST request to a webhook receiving form submission data.

## Process Summary
The workflow has two main paths: one for scheduled tweet processing and another for real-time form submissions. For tweets, it searches for specific keywords on Twitter, extracts relevant information, and filters out retweets or old content. For form submissions, it extracts content from the incoming webhook data. Both paths then perform sentiment analysis using Google Cloud Natural Language on the extracted text. If the sentiment is positive (score above 0.3 for tweets, 0.4 for form submissions), the content is prepared for storage.

## Output Details
The workflow stores positively-rated tweets or form submissions as new posts in a Strapi CMS.

## Tags
automation,n8n,production-ready,excellent,optimized
