# Workflow Analysis for Automated WhatsApp Message Processing and Database Update

## Description
This workflow automates the processing of incoming WhatsApp messages, analyzes their content to determine sentiment, translates messages, generates AI responses, and updates a Google Sheet with conversation details.

## Input Details
The workflow is triggered by incoming WhatsApp messages via a webhook.

## Process Summary
The workflow starts by receiving a WhatsApp message. It then processes the message for sentiment analysis using an external API, and translates the message using another API. If the message is in Spanish, it skips translation. Afterward, it generates an AI response based on the message content and sentiment. Finally, it formats the conversation data and appends it to a Google Sheet.

## Output Details
The workflow updates a Google Sheet named "Base de datos conversas" with the processed WhatsApp messages, AI responses, and sentiment analysis results.
