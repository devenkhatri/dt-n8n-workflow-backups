# Workflow Analysis for Fun AI Chat

## Description
This workflow provides a humorous AI chatbot that responds to user messages with funny and light-hearted replies in a mix of English, Hindi, or Gujarati, without referencing past conversation history.

## Input Details
The workflow is triggered by a POST request to a webhook endpoint containing a JSON payload with 'message' and optional 'history' fields.

## Process Summary
The workflow starts with a webhook receiving a user message. The message is passed to an AI Agent configured to generate funny, unique responses while ignoring conversation history. The AI Agent uses a Groq-hosted GPT-oss-120b language model to generate the reply. The response is then sent back to the webhook caller via the Respond to Webhook node.

## Output Details
The workflow returns a humorous AI-generated message directly as the HTTP response to the webhook request.

## Tags
AI, chatbot, webhook, humor, multilingual, Groq, GPT
