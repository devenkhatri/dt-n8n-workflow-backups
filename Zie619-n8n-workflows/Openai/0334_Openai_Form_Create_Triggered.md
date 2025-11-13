# Workflow Analysis for Customer Feedback Sentiment Analysis and Google Sheets Recording

## Description
This workflow automates the collection of customer feedback, performs sentiment analysis using OpenAI, and then records the feedback along with its sentiment in Google Sheets.

## Input Details
The workflow is triggered by a form submission where customers provide their name, feedback category, feedback text, and contact information.

## Process Summary
First, a customer submits feedback through a form. Next, the customer's feedback text is sent to OpenAI to classify its sentiment. Then, the original form data and the sentiment analysis result from OpenAI are merged together. Finally, this combined information, including timestamp, category, customer feedback, name, contact, and sentiment, is appended as a new row to a Google Sheet.

## Output Details
The workflow updates a Google Sheet with new rows containing the customer's feedback, category, contact information, submission timestamp, and the sentiment analysis result from OpenAI.

## Tags
customer feedback, sentiment analysis, OpenAI, Google Sheets, form, automation, data management
