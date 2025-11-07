# Workflow Analysis for Automated Lemlist Reply Categorization and Slack Notification

## Description
This workflow automatically processes replies to Lemlist campaigns. It uses AI to categorize each reply (e.g., Interested, Unsubscribe, Out of office) and sends a detailed alert to a designated Slack channel. Based on the categorization, it can also automatically unsubscribe leads or mark them as interested within Lemlist to streamline outreach efforts.

## Input Details
The workflow is triggered by new replies received in Lemlist campaigns and receives data related to the replied email, sender, campaign, and lead.

## Process Summary
Upon receiving a new Lemlist email reply, the workflow first cleans the reply text using Markdown. It then sends this cleaned text to an OpenAI model, which classifies the reply into categories like "Interested," "Unsubscribe," or "Not interested." The workflow then routes the processed reply: all replies trigger a detailed Slack notification. Additionally, if a reply is categorized as "Unsubscribe," the lead is automatically unsubscribed in Lemlist, and if "Interested," the lead is marked as interested in Lemlist.

## Output Details
The workflow sends formatted alerts to a Slack channel, automatically unsubscribes leads from Lemlist campaigns, or marks leads as interested in Lemlist, depending on the AI's classification.
