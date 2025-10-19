# Workflow Analysis for AI-Powered Customer Review Sentiment Analysis and Slack Alert

## Description
This workflow is designed to automate customer feedback management. It receives new customer reviews, uses an AI model to analyze the sentiment of the text, and sends an instant notification to a team communication channel for any reviews classified as negative or critical, ensuring immediate attention to customer issues.

## Input Details
The workflow is initiated by a Webhook trigger, which is configured to receive structured data containing a new customer review or feedback entry.

## Process Summary
The workflow starts with a Webhook trigger to ingest the customer review data. A Code node is used to reliably extract and format the review text. An OpenAI node then performs a sentiment classification on the text, categorizing it as positive, neutral, or negative. An IF node evaluates the classification result, routing the flow to the next steps only if the sentiment is "Negative". Finally, a Slack node posts a high-priority notification to a designated support channel with the review details.

## Output Details
The workflow produces an alert message sent to a specified Slack channel if the review sentiment is negative, and also returns a successful response to the triggering system.
