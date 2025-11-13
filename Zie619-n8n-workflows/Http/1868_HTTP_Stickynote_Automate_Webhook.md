# Workflow Analysis for Chatbot AI

## Description
This automated workflow integrates various services like webhooks, HTTP requests, and AI agents to provide an intelligent chatbot experience on Line, optimized for production with robust error handling and security.

## Input Details
The workflow is triggered by a webhook from Line, receiving incoming chat events which include user messages and other event details.

## Process Summary
The workflow initiates by sending a loading animation to the user on Line. It then checks if the incoming message is text; if not, it replies that the input type is unsupported. If the message is text, an AI Agent, configured as a CBT therapist, processes the message using an Azure OpenAI Chat Model. The AI-generated response is then formatted to remove special characters and sent back to the user on Line.

## Output Details
The workflow sends a text message reply to the user via the Line messaging platform, which is either an AI-generated therapeutic response or a message indicating unsupported input types.

## Tags
automation, n8n, production-ready, excellent, optimized
