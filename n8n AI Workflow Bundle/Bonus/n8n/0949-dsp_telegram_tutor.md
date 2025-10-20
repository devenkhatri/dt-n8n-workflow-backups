# Workflow Analysis for Telegram AI Chatbot Tutor

## Description
This workflow creates an AI-powered chatbot tutor on Telegram that provides instant answers and expands on topics based on user questions. It leverages OpenAI for generating responses and maintaining conversation history.

## Input Details
The workflow is triggered by an incoming message to a Telegram bot.

## Process Summary
The workflow receives a Telegram message and retrieves the user ID. It then fetches previous conversation history from a Google Sheet. It constructs a prompt for OpenAI, including the system message and conversation history, to generate a relevant response. Finally, it sends the AI-generated response back to the user on Telegram and updates the conversation history in the Google Sheet.

## Output Details
The workflow sends AI-generated textual responses to the user via Telegram and stores conversation history in a Google Sheet.
