# Workflow Analysis for Lemlist Reply Categorization and Slack Notification

## Description
This workflow automates the processing of new email replies from Lemlist campaigns. It uses AI to classify each reply and then performs actions such as sending a detailed alert to a Slack channel, unsubscribing leads who wish to opt-out, or marking leads as interested within Lemlist.

## Input Details
The workflow is triggered by new email replies from Lemlist campaigns, receiving details about the sender, lead, campaign, and the email text.

## Process Summary
1. Upon receiving a new reply from a Lemlist campaign, the workflow first formats the email text. 2. An AI model (OpenAI) then classifies the reply into predefined categories such as "Interested," "Unsubscribe," or "Not Interested." 3. The classified reply data is merged with the original Lemlist data. 4. Based on the categorization, the workflow routes the reply to different branches for specific actions. 5. Finally, a structured alert containing reply details and its category is sent to a designated Slack channel.

## Output Details
The workflow produces a categorized Slack alert for each new reply, and optionally unsubscribes leads or marks them as interested within Lemlist based on the reply's content.

## Tags
Lemlist, Email, Reply Management, AI Categorization, Slack, Automation, Lead Management, OpenAI, Unsubscribe, Sales Workflow
