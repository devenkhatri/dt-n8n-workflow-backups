# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using an AI sales agent to answer queries, qualify leads, and potentially close sales.

## Input Details
The workflow is triggered by an incoming message to a WhatsApp business account, receiving the message content and sender information.

## Process Summary
First, the workflow checks if the incoming message contains media. If it does, a default "I can only process text messages" response is sent via WhatsApp. If not, the message is sent to an AI assistant (OpenAI Chat) to generate a response. The AI assistant is configured with a system prompt outlining its role as a sales agent and provided with a summary of the current conversation history. After getting the AI response, the workflow extracts the message content and sends it back to the customer via WhatsApp. Finally, the entire conversation, including the AI's response, is logged in a Google Sheet to maintain a record of interactions.

## Output Details
The workflow responds to the customer on WhatsApp with an AI-generated message or a predefined message regarding media content, and logs the conversation in a Google Sheet.
