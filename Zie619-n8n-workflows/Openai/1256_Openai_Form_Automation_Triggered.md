# Workflow Analysis for Customer Feedback Sentiment Analysis

## Description
This workflow automates the process of collecting customer feedback, analyzing its sentiment using OpenAI, and storing the categorized and sentiment-analyzed feedback in Google Sheets for easy tracking and analysis.

## Input Details
The workflow is triggered by a customer submitting a feedback form, which collects details such as customer name, feedback category, the feedback itself, and contact information.

## Process Summary
First, a customer submits feedback through a dedicated form. Then, the submitted feedback text is sent to OpenAI to determine its sentiment. Afterward, the original feedback form data is merged with the sentiment analysis result from OpenAI. Finally, this combined data, including customer details, feedback category, raw feedback, timestamp, and the determined sentiment, is appended as a new row to a Google Sheet.

## Output Details
The workflow creates a new row in a Google Sheet, populating it with the customer's feedback, their contact information, the feedback category, the submission timestamp, and the sentiment determined by OpenAI.

## Tags
Customer Feedback, Sentiment Analysis, OpenAI, Google Sheets, Form Submission, Automation
