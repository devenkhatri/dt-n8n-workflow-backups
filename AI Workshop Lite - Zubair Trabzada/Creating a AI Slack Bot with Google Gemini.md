# Workflow Analysis for Slack AI Assistant with Memory

## Description
This workflow receives messages from Slack via a webhook, processes them using an AI assistant powered by Google Gemini, remembers conversation history using session-based memory, and sends the AI's response back to the same Slack channel.

## Input Details
The workflow is triggered by a POST webhook that receives incoming messages from Slack, including message text, user name, channel ID, and a token used for session memory.

## Process Summary
The workflow starts by receiving a Slack message through a POST webhook. The message text is passed to an AI agent configured with a system prompt and powered by the Google Gemini model. Conversation history is maintained using a window buffer memory, keyed by the Slack message token to preserve context per session. The AI processes the input and generates a response. Finally, the response is formatted and sent back to the original Slack channel as a new message.

## Output Details
The workflow sends the AI-generated response back to the Slack channel where the original message was posted, mentioning the original user and showing the bot's reply.

## Tags
Slack, AI Assistant, Webhook, Google Gemini, Memory, Chatbot, Automation
