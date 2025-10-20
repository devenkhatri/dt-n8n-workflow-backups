# Workflow Analysis for Automated Feedback Analysis with AI and Google Sheets Integration

## Description
This workflow automates the process of collecting feedback from a webhook, analyzing its sentiment using either OpenAI or Google AI, and then storing the results, including the sentiment score, in a Google Sheet.

## Input Details
The workflow is triggered by an incoming webhook that provides feedback data.

## Process Summary
The workflow starts by receiving feedback data from a webhook. It then determines whether to use OpenAI or Google AI for sentiment analysis based on a condition. The chosen AI model analyzes the feedback and assigns a sentiment score. Finally, the original feedback along with the sentiment score is appended as a new row in a specified Google Sheet.

## Output Details
The workflow outputs the sentiment analysis results by adding a new row with the feedback text and sentiment score to a Google Sheet.
