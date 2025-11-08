# Workflow Analysis for Telegram-bot AI Da Nang

## Description
This workflow powers an AI chatbot for the Da Nang meetup group, enabling it to answer questions about the group's schedule by retrieving information from a Google Sheet and processing queries using a large language model.

## Input Details
The workflow is triggered by either a new chat message received from Telegram or a chat input within the n8n environment itself.

## Process Summary
First, the workflow normalizes the incoming chat message and identifies the source (Telegram or n8n). Then, it retrieves schedule data from a Google Spreadsheet, converting it into a markdown table. This markdown table, along with the user's message, is fed to an AI agent that uses a language model and chat memory to generate a relevant response. Finally, the AI-generated response is assembled and routed back to the appropriate chat platform.

## Output Details
The workflow responds by sending the AI-generated answer back to the originating chat platform, either Telegram or the n8n chat interface.
