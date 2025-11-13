# Workflow Analysis for Analyze the sentiment of feedback and send a message on Mattermost

## Description
Automated workflow: Analyze the sentiment of feedback and send a message on Mattermost. This workflow processes data and performs automated tasks, optimized for production use with comprehensive error handling, security, and documentation.

## Input Details
The workflow is triggered by new submissions from a Typeform form, receiving feedback data.

## Process Summary
The workflow is initiated by new feedback submissions from a Typeform form. It then uses Google Cloud Natural Language to analyze the sentiment of the submitted feedback, obtaining a sentiment score. An 'If Node' checks this sentiment score against a predefined condition. If the condition is met, a message containing the feedback and its sentiment score is posted to a specified Mattermost channel. Otherwise, no further action is taken for that feedback, and an error handler is available for execution failures.

## Output Details
The workflow sends a message containing the feedback and its sentiment score to a designated Mattermost channel if the sentiment meets a specified condition.

## Tags
automation, n8n, production-ready, excellent, optimized, Typeform, Google Cloud Natural Language, Mattermost, sentiment analysis, feedback
