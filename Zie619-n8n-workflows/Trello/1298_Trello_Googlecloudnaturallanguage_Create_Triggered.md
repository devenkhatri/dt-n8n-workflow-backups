# Workflow Analysis for Typeform Feedback Processing Workflow

## Description
This workflow automates the processing of feedback submitted through a Typeform, analyzes its sentiment using Google Cloud Natural Language, and then routes the feedback to either Notion and Slack for positive sentiment or Trello for negative or neutral sentiment.

## Input Details
The workflow is triggered by new submissions to a specific Typeform, receiving form data including the submitter's name and their suggestions.

## Process Summary
1. The workflow is initiated when a new response is submitted to a Typeform. 2. It then extracts the submitted suggestion text and sends it to Google Cloud Natural Language for sentiment analysis. 3. An If node evaluates the sentiment score provided by Google Cloud Natural Language. 4. If the sentiment score is positive, the feedback details (name and suggestion) are recorded in Notion and a notification is sent to a specified Slack channel. 5. If the sentiment score is zero or negative, a new card is created in Trello containing the feedback and sentiment score.

## Output Details
The workflow either creates a new page in Notion and sends a message to Slack for positive feedback, or it creates a new card in Trello for neutral or negative feedback.

## Tags
Typeform, Sentiment Analysis, Google Cloud Natural Language, Notion, Slack, Trello, Feedback Processing, Automation
