# Workflow Analysis for Bitrix24 Chatbot Application with Webhook Integration

## Description
This workflow integrates a Bitrix24 chatbot with a custom application using webhooks, allowing for interactive conversations and data exchange.

## Input Details
The workflow is triggered by an HTTP webhook that receives message data from a Bitrix24 chatbot.

## Process Summary
The workflow starts by extracting relevant message text and user information from the incoming webhook data. It then checks if the message is a command to display existing tasks. If so, it fetches tasks from Bitrix24 and formats them for display. Otherwise, it interacts with an external application via another webhook, sending the user message and receiving an AI-generated response. Finally, it sends the processed information or AI response back to the Bitrix24 chatbot for the user.

## Output Details
The workflow sends formatted messages, task lists, or AI-generated responses back to the Bitrix24 chatbot.
