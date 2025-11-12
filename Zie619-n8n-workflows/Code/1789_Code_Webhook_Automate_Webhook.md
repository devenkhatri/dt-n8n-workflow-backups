# Workflow Analysis for (G) LineChatBot + Google Sheets (as a memory)

## Description
This workflow powers a Thai-language AI chatbot integrated with LINE Messenger that remembers conversation history by storing it in Google Sheets. It retrieves past interactions for context-aware responses and sends replies back to users via LINE’s API.

## Input Details
The workflow is triggered by a POST request to a webhook endpoint from LINE Messenger containing user message data.

## Process Summary
1. The webhook receives a message from LINE Messenger and extracts the user ID, message text, and reply token. 2. It fetches the user's conversation history from a Google Sheet using the user ID. 3. The AI prompt is constructed using past conversation history and the new user message. 4. Google Gemini generates a contextual response in Thai. 5. The new message-response pair is appended to the history, split into manageable chunks if necessary, and saved back to Google Sheets before the response is sent to the user via LINE’s API.

## Output Details
The workflow sends a personalized AI-generated message back to the user on LINE Messenger and updates the user's chat history in Google Sheets.

## Tags
LINE Chatbot, Google Sheets, AI Assistant, Conversation Memory, Google Gemini, Thai Language, Webhook Integration, Chat History, n8n Automation
