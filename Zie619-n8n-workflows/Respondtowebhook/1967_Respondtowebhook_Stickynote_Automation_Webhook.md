# Workflow Analysis for InstaTest

## Description
This workflow serves as the core component of an Instagram bot solution. It receives new messages from Instagram via ManyChat, generates responses using ChatGPT, and then sends the generated messages back to ManyChat for delivery to Instagram.

## Input Details
The workflow is triggered by a webhook that receives message data from Instagram, typically forwarded by ManyChat, containing a session ID and the chat input text.

## Process Summary
First, the workflow receives a message from Instagram via a webhook. It then configures a system prompt for an AI, identifying it as an Instagram influencer, and extracts the session ID and chat input. Next, an AI agent, leveraging a ChatGPT model and local n8n memory for message history, processes the chat input based on the defined prompt to generate a suitable response. Finally, the generated AI response is sent back.

## Output Details
The workflow produces an AI-generated text response to the incoming Instagram message, which is then sent back to ManyChat to be delivered to Instagram.

## Tags
Instagram, ManyChat, AI, ChatGPT, Chatbot, Webhook, Automation, Social Media
