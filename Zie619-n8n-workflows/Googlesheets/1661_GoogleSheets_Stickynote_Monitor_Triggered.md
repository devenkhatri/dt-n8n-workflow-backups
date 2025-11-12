# Workflow Analysis for AI agent: expense tracker in Google Sheets and n8n chat

## Description
This workflow allows users to send expense messages via an n8n chat interface, which are then parsed by an AI model into structured data (cost, description, date) and automatically saved as a new row in a Google Sheet.

## Input Details
The workflow is triggered when a user sends a chat message containing expense details (e.g., 'car wash; 59.3 usd; 25 jan 2024').

## Process Summary
When a chat message is received, it is passed to an AI agent powered by OpenAI. The agent uses a sub-workflow to extract structured JSON data (cost, description, and date) from the raw message. This structured data, along with the original message, is then appended as a new row to a specified Google Sheet. The AI responds to the user confirming the expense was saved and includes the parsed data. Error handling is in place to manage failures during execution.

## Output Details
The parsed expense data is saved as a new row in a Google Sheet, and a confirmation message with the structured data is returned to the user in the chat.

## Tags
AI agent, expense tracking, Google Sheets, n8n chat, OpenAI, automation, production-ready, JSON parsing, workflow automation
