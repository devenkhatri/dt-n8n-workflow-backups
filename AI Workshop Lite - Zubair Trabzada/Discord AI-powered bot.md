# Workflow Analysis for Discord AI bot

## Description
This workflow automatically analyzes user feedback messages using AI, categorizes them into 'success-story', 'urgent-issue', or 'ticket', and forwards them to the appropriate department via Discord webhooks.

## Input Details
The workflow is triggered by a POST request to a webhook endpoint containing user feedback in the 'feedback' field of the request body.

## Process Summary
The workflow receives user feedback via a webhook, sends it to OpenAI's GPT-4 model with instructions to categorize the message and generate a summary for the relevant team. The AI response is parsed from JSON format, and a switch node routes the message to the appropriate Discord channel—User Success, IT, or Helpdesk—based on the category. If the category doesn't match any expected values, it defaults to a 'do nothing' node.

## Output Details
The workflow sends a formatted instruction message to one of three Discord channels (User Success, IT, or Helpdesk) based on the AI-determined category of the user feedback.

## Tags
AI, Discord, automation, customer support, categorization, webhook, OpenAI, GPT-4, routing, feedback
