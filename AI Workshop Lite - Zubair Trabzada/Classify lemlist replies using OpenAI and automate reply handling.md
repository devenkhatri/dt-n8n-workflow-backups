# Workflow Analysis for Lemlist Reply Handler with AI Categorization and Slack Alerts

## Description
This workflow automatically processes email replies from Lemlist campaigns by categorizing them using AI, sending detailed alerts to a Slack channel, and taking follow-up actions like unsubscribing uninterested leads or marking interested ones directly in Lemlist.

## Input Details
The workflow is triggered by new email replies in Lemlist campaigns via a webhook.

## Process Summary
When a new reply is received from Lemlist, the workflow first cleans and formats the reply text using Markdown. It then sends the cleaned text to OpenAI's GPT-4o model to classify the reply into one of five categories: Interested, Out of office, Unsubscribe, Not interested, or Other. The classification result is merged with the original reply data. Based on the category, the workflow routes the reply to different branches: it always sends a formatted alert to a Slack channel, automatically unsubscribes leads who requested to opt-out, and marks interested leads as such in Lemlist.

## Output Details
The workflow sends a structured Slack message with reply details and category, unsubscribes leads who reply with 'Unsubscribe', and marks 'Interested' leads as such in Lemlist.

## Tags
lemlist, slack, openai, email replies, lead management, automation, ai categorization, unsubscribe, interested leads
