# Workflow Analysis for AI Personal Assistant for Telegram

## Description
An AI-powered personal assistant that responds to user requests via Telegram by accessing emails, calendar events, tasks, and contacts to provide helpful, contextual information.

## Input Details
The workflow is triggered by incoming messages or voice notes from users in Telegram.

## Process Summary
The workflow first receives a message or voice note from Telegram. If it's a voice note, it downloads the audio file and converts it to text using OpenAI's speech-to-text. The text is then passed to an AI assistant powered by OpenAI's GPT-4o-mini, which has access to the user's Gmail, Google Calendar, Baserow tasks, and contacts. The assistant follows guidelines to fetch and summarize relevant data based on the user’s request, maintaining conversation context using window buffer memory. Finally, the assistant's response is sent back to the user via Telegram.

## Output Details
The workflow sends a formatted response message back to the user in Telegram containing the requested information or action result.

## Tags
AI assistant, Telegram bot, Gmail integration, Google Calendar, Baserow, speech-to-text, personal assistant, automation
