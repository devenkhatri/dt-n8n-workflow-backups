# Workflow Analysis for Automate Lemlist Reply Classification and Actions with Slack Alerts

## Description
This workflow automates the processing of replies from Lemlist email campaigns. It classifies each reply using AI, sends an informative alert to a Slack channel, and performs automated actions within Lemlist based on the reply's category, such as unsubscribing leads or marking them as interested.

## Input Details
The workflow is triggered by new email replies received in a Lemlist campaign, providing reply text and lead details.

## Process Summary
1. Upon receiving a new Lemlist email reply, the workflow first cleans the reply text.
2. It then uses an OpenAI model to classify the reply into categories like "Interested," "Unsubscribe," "Out of office," "Not interested," or "Other."
3. The workflow merges the original Lemlist data with the AI-generated category.
4. Based on the classified category, it routes the workflow to different branches.
5. Regardless of the category, a detailed alert is sent to a specified Slack channel, including the category, campaign information, and a reply preview.
6. If the reply is categorized as "Unsubscribe," the lead is automatically unsubscribed in Lemlist.
7. If the reply is categorized as "Interested," the lead is marked as interested in Lemlist.

## Output Details
The workflow sends structured alerts to a Slack channel and performs actions within Lemlist, specifically unsubscribing leads or marking them as interested, based on the AI classification.
