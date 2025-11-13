# Workflow Analysis for Lemlist Reply Classification and Slack Notification Workflow

## Description
This automated workflow processes new replies from Lemlist email campaigns, categorizes them using an AI model, and then takes appropriate actions such as sending notifications to Slack and updating lead statuses in Lemlist.

## Input Details
The workflow is triggered by new email replies received from Lemlist campaigns.

## Process Summary
Upon receiving a new reply from a Lemlist campaign, the workflow formats the email text. It then uses an OpenAI model to classify the reply into categories like "Interested", "Unsubscribe", or "Not interested". The categorized reply and original data are merged. Subsequently, a detailed alert is sent to a specified Slack channel, providing insights into the reply. If the reply is categorized as "Unsubscribe", the lead is automatically unsubscribed in Lemlist; if classified as "Interested", the lead is marked as interested in Lemlist.

## Output Details
The workflow sends a detailed, categorized alert to a Slack channel and, depending on the reply classification, either unsubscribes a lead or marks them as interested in Lemlist.

## Tags
automation, lemlist, slack, AI, email classification, lead management, customer engagement
