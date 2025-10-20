# Workflow Analysis for Workflow to Process Webhook Data and Generate AI Responses

## Description
This workflow processes incoming webhook data, extracts the user question, generates an AI response, summarizes the response, and then sends both the summarized and full AI responses via a webhook.

## Input Details
The workflow is triggered by a webhook and receives data in JSON format.

## Process Summary
The workflow starts by extracting the user's question from the incoming webhook data. It then generates an AI response based on this question. Next, it summarizes the generated AI response. Finally, it combines the original user's question and both the summarized and full AI responses before sending them as a payload to another webhook.

## Output Details
The workflow sends a POST request with the user's question, the summarized AI response, and the full AI response to a specified webhook URL.
